FROM node:latest

ENV ELECTRON_DISABLE_SANDBOX=true

RUN apt-get update && \
    apt-get install -y \
        libgtk3.0 \
        libgconf-2-4 \
        libasound2 \
        libxtst6 \
        libxss1 \
        libnss3 \
        xvfb
