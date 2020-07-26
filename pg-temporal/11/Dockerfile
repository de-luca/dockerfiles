FROM postgres:11-alpine

RUN apk add --no-cache --virtual build-deps musl-dev make gcc git clang llvm && \
    git clone --single-branch --branch mlt https://github.com/mlt/temporal_tables.git --depth 1 && \
    cd temporal_tables && \
    make && \
    make install && \
    apk del build-deps
