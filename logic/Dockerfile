FROM mcr.microsoft.com/dotnet/sdk:7.0 as build-env
WORKDIR /SoundUNder_library_ms
COPY SoundUNder_library_ms/*.csproj .
RUN dotnet restore
COPY * .
RUN dotnet add package MongoDB.Driver
RUN dotnet publish -c Release -o /publish

FROM mcr.microsoft.com/dotnet/aspnet:7.0 as runtime
WORKDIR /publish
COPY --from=build-env /publish .
EXPOSE 80
ENTRYPOINT ["dotnet", "sistema_library_ms.dll"]