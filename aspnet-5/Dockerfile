FROM mcr.microsoft.com/dotnet/aspnet:5.0-focal
RUN groupadd -g 1000 app && useradd app -u 1000 -g 1000 -m -s /usr/sbin/nologin
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y && apt-get install -y curl && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /var/cache/apt/archives/* /var/cache/debconf/*-old
USER app
ENV ASPNETCORE_HTTP_PORTS=8080
ENV ASPNETCORE_URLS=http://+:8080
ENV DOTNET_URLS=http://+:8080
EXPOSE 8080
WORKDIR /app
HEALTHCHECK --interval=1m --timeout=3s CMD curl -f http://localhost:8080/healthz || exit 1
