ogmios-nix-docker
=================

Builds [CardanoSolutions/ogmios](https://github.com/CardanoSolutions/ogmios)
using Nix infra based on
[input-output-hk/cardano-ogmios](https://github.com/input-output-hk/cardano-ogmios).

Adds a Nix-built Docker image.
Only builds a standalone `ogmios` image so far, not `cardano-node-ogmios`.

Usage:

```
nix build .#dockerImage
docker load < result
docker image ls jefdaj/ogmios-nix-docker
```
