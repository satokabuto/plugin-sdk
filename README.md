kintone Plug-in SDK
==========================

This SDK includes kintone plug-in packaging tool.

## Requirement

* A bash shell
* zip and openssl libraries are required using Cygwin on Windows


## How to Use

```bash
$ package.sh <plug-in dir> [<key file>]
```
## Output Files

### Plug-in Package
```bash
plugins/<plug-in id>/plugin.zip
```

### Private Key
```bash
keys/<plug-in dir>.<plug-in id>.ppk
```
**Do not lose the private key!** Keep the .ppk file secret and in a safe place. You'll need it later if you want to update the plug-in.

## Example
```bash
$ cd /tmp
$ git clone https://github.com/kintone/plugin-sdk
$ cd plugin-sdk
$ ./package.sh examples/colorcell
Plugin ID: lnamdpliafiofedbofmbgijdjpgebobo
Plugin file: /tmp/plugin-sdk/plugins/lnamdpliafiofedbofmbgijdjpgebobo/plugin.zip
Private key file: /tmp/plugin-sdk/keys/colorcell.lnamdpliafiofedbofmbgijdjpgebobo.ppk
```

## Licence

GPL v2

## Copyright

Copyright(c) Cybozu, Inc.