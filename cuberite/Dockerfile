FROM alpine:3.6 AS wget
RUN apk add --no-cache ca-certificates wget tar

FROM wget AS cuberite
ARG CUBERITE_BUILD=1013
WORKDIR /srv
RUN wget -qO- "https://builds.cuberite.org/job/Cuberite Linux x64 Master/${CUBERITE_BUILD}/artifact/Cuberite.tar.gz" \
    | tar -xzf -

FROM debian:jessie
RUN apt-get update; apt-get install -y ca-certificates
COPY --from=cuberite /srv /srv
EXPOSE 25565 8080
WORKDIR /srv/Server
ENTRYPOINT ["/srv/Server/Cuberite"]