# VeChain Sync client install and verify script

## Reads Sync client install data from:
 - https://env.vechain.org and https://github.com/vechain/
 - https://github.com/vechain/thor-sync.electron

## Actions
- Compare version, checksum, and metadata from both sources
- Download latest github release AppImage binary
- Compute SHA512 checksum of downloaded binary
- encodes SHA522 output as base64 to match mechanism used by VeChain
- Verify calculated checksum against published (webpage and github) checksums
- On validation success, install AppImage to ~/Desktop
