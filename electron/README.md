# Electron

[![Docker Pulls](https://img.shields.io/docker/pulls/deluca/electron.svg)](https://hub.docker.com/r/deluca/electron/)

See https://github.com/jprichardson/electron-mocha/issues/95#issuecomment-270222421

*I use this image for testing and local dev (headless).*

## Base image
`node:latest`

## Included packages
Required libs to run headless test using [electron-mocha](https://github.com/jprichardson/electron-mocha).

- libgtk3.0
- libgconf-2-4
- libasound2
- libxtst6
- libxss1
- libnss3
- xvfb

## Env
`ELECTRON_DISABLE_SANDBOX=true` to prevent the sandbox error.

## Usage
```sh
xvfb-run --server-args=$XVFB_ARGS electron-mocha [...]
```
```sh
xvfb-run --server-args="-screen 0 1024x780x24" [nyc] electron-mocha [...]
```
