FROM mcr.microsoft.com/dotnet/aspnet:5.0-focal
RUN addgroup -S app && adduser -S app -G app
USER app
ENV ASPNETCORE_HTTP_PORTS=8080
ENV ASPNETCORE_URLS=http://+:8080
ENV DOTNET_URLS=http://+:8080
EXPOSE 8080
WORKDIR /app
