pangea-electron
==============

forked from [patchwork-electron](https://github.com/ssbc/patchwork-electron)

## Running from source

```bash
$ cd ~
$ git clone https://github.com/Bit-Nation/pangea-electron.git
$ cd pangea-electron
$ npm install
$ npm start
```

To use the latest patchwork version, do the following:

```bash
$ cd ~
$ git clone https://github.com/Bit-Nation/pangea.git
$ cd pangea
$ npm install
$ npm link
$ cd ~/pangea-electron/app
$ npm link pangea
```

## Troubleshooting

If you get an error similar to:

> Uncaught Exception:
> Error: Module version mismatch. Expected 50, got 48.

It means your installed node version is not compatible with the version of Electron pangea uses. You'll need to rebuild your node module folder using:

```bash
$ npm run rebuild
```

## Building

```bash
$ npm run release
```

## More info

This repo is based on https://github.com/szwacz/electron-boilerplate.
Check that repo to get more information on the structure and scripts.
