# Electron

[![Docker Pulls](https://img.shields.io/docker/pulls/deluca/electron.svg)](https://hub.docker.com/r/deluca/electron/)

See https://github.com/jprichardson/electron-mocha/issues/95#issuecomment-270222421

## Includes
Required libs to run headless test using [electron-mocha](https://github.com/jprichardson/electron-mocha) for libs for [Electron](https://electron.atom.io).

## Usage
```sh
xvfb-run --server-args=$XVFB_ARGS electron-mocha [...]
```
