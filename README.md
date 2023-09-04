# P256 Signer

## Contracts overview

### FCL/FCL_elliptic.sol

The `FCL_Elliptic_ZZ` library implements computation of ECDSA verification using the secp256r1 curve.It uses a [XYZZ system coordinates](https://hyperelliptic.org/EFD/g1p/auto-shortw-xyzz.html).
This contract is from [here](https://github.com/rdubois-crypto/FreshCryptoLib/tree/master). The original repository also contains tests.

### Webauthn.sol

The `Webauthn` library implements the decoding and verification of a signed Webauthn payload.

### P256Signer.sol

The `P256Signer` contract represents a Gnosis Safe signer for a given secp256r1 public key.

### P256SignerFactory.sol

The `P256SignerFactory` contract is a factory for P256Signers. It allows us to have deterministic addresses for a given secp256r1 public key.