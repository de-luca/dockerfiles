FROM ubuntu:zesty

RUN apt-get update &&\
    apt-get install -y curl gcc make curl libpq-dev

RUN curl https://sh.rustup.rs -sSf | sh -s -- -y --default-toolchain nightly &&\
    tail -1 ~/.profile >> ~/.bashrc

WORKDIR /source
