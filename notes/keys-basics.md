# Secret Key vs Public/Private Key

This note explains the difference between a **secret key** system and a **public/private key** system.

## 1) Secret Key (Symmetric Encryption)

- One shared key is used to both encrypt and decrypt data.
- Both sender and receiver must keep the same key secret.
- Fast and efficient for large data.

### Main challenge

- Securely sharing that one key with another party.

### Common uses

- Encrypting files at rest
- Encrypted sessions after key exchange (for performance)

## 2) Public / Private Key (Asymmetric Encryption)

- You have a key pair:
  - **Public key**: can be shared with anyone
  - **Private key**: must stay secret
- Data encrypted with the public key can only be decrypted with the private key.
- Data signed with the private key can be verified with the public key.

### Main advantages

- Solves key distribution problem (public key can be openly shared)
- Enables digital signatures and identity verification

### Common uses

- TLS/HTTPS handshakes
- SSH authentication
- Signing software and documents

## Quick Comparison

| Topic | Secret Key | Public/Private Key |
|---|---|---|
| Number of keys | 1 shared key | 2 keys (public + private) |
| Speed | Usually faster | Usually slower |
| Key sharing | Harder (must be secure) | Easier (public key is shareable) |
| Digital signatures | Not ideal | Supported |
