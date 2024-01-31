FROM mcr.microsoft.com/dotnet/aspnet:5.0-focal
RUN groupadd -g 1000 app && useradd app -u 1000 -g 1000 -m -s /usr/sbin/nologin
USER app
ENV ASPNETCORE_HTTP_PORTS=8080
ENV ASPNETCORE_URLS=http://+:8080
ENV DOTNET_URLS=http://+:8080
EXPOSE 8080
WORKDIR /app
