# About
Subkey is a public key cryptographic utility that is developed within [Substrate][1] itself. Its main feature is generating and inspecting key pairs, currently supporting these scheme:

sr25519: Schorr signatures on the Ristretto group
ed25519: SHA-512 (SHA-2) on Curve25519
secp256k1: ECDSA signatures on secp256k1

All keys in Substrate based networks (like polkadot) use the SS58 address encoding format that is the primary user-facing way to interact with keys.

Subkey also allows restoring keys from mnemonics and raw seeds; signing and verifying signatures on a message; and signing and verifying signatures for encoded transactions.

This is a simple dockerfile for create a docker image with subkey.

# Requirements

`Docker`

# How to execute

Build image: 
`docker build ./ -f Dockerfile-subkey -t rayniel95/substrate/subkey:v1.0`

Execute container: `docker run rayniel95/substrate/subkey:v1.0 subkey -h`

# How to use
Follow the instructions with the `-h` command.

[1]: https://github.com/paritytech/substrate