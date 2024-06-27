# publish
FROM mcr.microsoft.com/dotnet/sdk:7.0.400 AS build

WORKDIR /app

COPY src/ .

RUN dotnet publish -c Release -o out

# run
FROM mcr.microsoft.com/dotnet/aspnet:7.0

WORKDIR /app

COPY --from=build /app/out .

ENTRYPOINT ["dotnet", "PizzaStore.dll"]
