# Use the official .NET SDK image for build
FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build
WORKDIR /src

# Copy project files and restore
COPY . . 
RUN dotnet restore "./Admin-Dashboard.csproj"

# Build the project
RUN dotnet publish "./Admin-Dashboard.csproj" -c Release -o /app/publish

# Use the official runtime image
FROM mcr.microsoft.com/dotnet/aspnet:7.0
WORKDIR /app
COPY --from=build /app/publish .

# Expose port
EXPOSE 80

# Start app
ENTRYPOINT ["dotnet", "Admin-Dashboard.dll"]
