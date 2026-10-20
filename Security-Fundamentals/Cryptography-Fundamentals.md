# Encryption

Encryption converts plaintext into ciphertext using an algorithm and a key, making the data unreadable to unauthorized parties.

- **Purpose:** Confidentiality.
- **Example:** AES encryption.

# Hashing

Hashing uses a hash function to convert data of any supported length into a fixed-length hash value (digest).

- **Purpose:** Integrity verification.
- **Examples:** SHA-256, SHA-3.
- Hashing is a one-way process; it is not designed to be decrypted.

# Symmetric Encryption

The same secret key is used for both encryption and decryption.

- **Advantages:** Fast and efficient for large amounts of data.
- **Example:** AES.

# Asymmetric Encryption

Asymmetric cryptography uses a pair of mathematically related keys:

- **Public key:** Can be shared publicly.
- **Private key:** Must be kept secret.

Depending on the algorithm and purpose, these keys can support encryption, key establishment, or digital signatures.

- **Examples:** RSA, ECC.

# Digital Signature

A digital signature helps verify data integrity and the authenticity of the signer. It can also support non-repudiation.

- The signer creates a signature using their private key.
- The recipient verifies the signature using the corresponding public key.
- A valid signature helps establish that the signed data has not been altered and that the signature corresponds to the associated private key.

# Digital Certificate

A digital certificate binds an identity to a public key and is typically issued and digitally signed by a trusted Certificate Authority (CA).

- **Purpose:** Helps establish trust in a public key and its associated identity.
- **Common use:** HTTPS/TLS certificates.
- A certificate's validity and trust depend on checks such as its signature, validity period, identity, and certificate chain.
