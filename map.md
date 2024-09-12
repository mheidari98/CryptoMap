---
title: Cryptography Roadmap for CTF
markmap:
  colorFreezeLevel: 5
---

## Classical Cryptography
  - **Permutation Ciphers**
    - ==Rearranges the letters or groups of letters in a message without changing them==
    - **Rail Fence Cipher**: Arranges text in a zigzag pattern on multiple lines and then reads it row by row.
    - **Columnar Transposition Cipher**: Writes the message in rows and reads it in columns according to a keyword.
  
  - **Substitution Ciphers**
    - ==Replaces each letter in the plaintext with another letter, often according to a fixed system==
    - **Caesar Cipher**: Shifts each letter by a fixed number in the alphabet.
    - **Vigenère Cipher**: Uses a keyword to determine shifts for each letter, making it harder to break.
    - **Atbash Cipher**: Reverses the alphabet (A = Z, B = Y, etc.).
    - **Playfair Cipher**: Uses a 5x5 grid of letters and digraphs to encrypt.
    - **Hill Cipher**: Encrypts letters in blocks using matrix multiplication with a key matrix.
  
  - **Polyalphabetic Ciphers**
    - ==A type of substitution cipher that uses multiple substitution alphabets to encrypt the message. It changes the substitution system at different points in the text, making it more resistant to frequency analysis==
    - **Vigenère Cipher**: Uses a keyword to determine shifts for each letter, applying a different substitution alphabet at each position.
    - **Beaufort Cipher**: Similar to the Vigenère Cipher but uses subtraction in place of addition during encryption.
    - **Example in Use:**
    - If the plaintext is "HELLO" and the key is "KEY", the letters are shifted based on the positions of "K", "E", and "Y", making it harder to detect patterns.
  
  - **Frequency Analysis Techniques**
    - A method used to crack substitution ciphers by analyzing how frequently certain letters appear in the ciphertext and comparing these frequencies to typical letter distributions in the language.
    - **Example**: In English, "E" is the most common letter. If the most frequent letter in the ciphertext is "Q", it might correspond to "E" in the plaintext.


## Modern Cryptography
### Symmetric Cryptography
  - **Stream Ciphers**
    - ==Encrypts data one bit or byte at a time==
    - ChaCha20
    - Salsa20
    - RC4
  - **Block Ciphers**
    - ==Encrypts data in fixed-size blocks (e.g., 64 or 128 bits)==
    - DES
    - 3DES
    - AES
    - Blowfish
    - Twofish
  - **Modes of Operation**
    - ==Techniques to securely encrypt large amounts of data==
    - ECB (Electronic Codebook)
    - CBC (Cipher Block Chaining)
    - CFB (Cipher Feedback)
    - OFB (Output Feedback)
    - CTR (Counter Mode)

### Asymmetric Cryptography
  - **RSA (Rivest–Shamir–Adleman)**
    - ==Relies on the difficulty of factoring large numbers==
  - **ElGamal**
  - **DSA (Digital Signature Algorithm)**
  - **ECC (Elliptic-Curve Cryptography)**
    - ==Based on algebraic structures of elliptic curves over finite fields==
    - Curve25519
    - P-256
  - **Diffie-Hellman Key Exchange**
    - ==Used for secure key exchange over an insecure channel==
  - **Post-Quantum Cryptography (NTRU, Lattice-based cryptography)**

## Hash Functions
  - **MD5**
  - **SHA-1**
  - **SHA-2 (SHA-256, SHA-512)**
  - **SHA-3 (Keccak)**
  - **HMAC (Hash-based Message Authentication Code)**
  - **BLAKE2**
  - **PBKDF2 (Password-Based Key Derivation Function 2)**
  - **bcrypt**
  - **Argon2**

## Public Key Infrastructure (PKI)
  - Certificates and Certificate Authorities (CA)
  - X.509 Standard
  - Digital Signatures
  - Key Management


## Cryptographic Protocols
  - TLS/SSL
  - SSH
  - PGP (Pretty Good Privacy)
  - IPSec
  - Kerberos
  - Zero-Knowledge Proofs

## Cryptanalysis Techniques
  - **Brute Force Attack**
    - ==Tries every possible key until the correct one is found.==
  - **Frequency Analysis (Classical Ciphers)**
    - ==Analyzes the frequency of letters or groups of letters to crack substitution ciphers==
  - **Known-plaintext Attack**
     - ==The attacker has access to both the plaintext and its corresponding ciphertext and uses this information to derive the key==
  - **Chosen-plaintext Attack**
    - ==The attacker can choose arbitrary plaintexts and obtain their corresponding ciphertexts, allowing them to gather information to break the encryption==
  - **Chosen-ciphertext Attack**
    - ==The attacker can decrypt chosen ciphertexts and use this to gain information about the encryption key or algorithm==
  - **Meet-in-the-Middle Attack (Block Ciphers)**
    - ==A known-plaintext attack that targets block ciphers by using a space-time tradeoff, working faster than brute force by exploiting the structure of two-key encryption schemes==
  - **Side-Channel Attacks**
    - ==Exploits physical leakages like timing or power consumption to break encryption==
    - **Timing Attacks**
      - ==Measures the time it takes to perform cryptographic operations to deduce secret keys==
    - **Power Analysis**
      - ==Monitors power consumption during encryption to extract information about the key==
  - **Differential Cryptanalysis**
    - ==Analyzes the differences in ciphertexts resulting from slight differences in the plaintext to discover the secret key==
  - **Linear Cryptanalysis**
    - ==Uses linear approximations to describe the behavior of block ciphers and analyzes the relationships between plaintext, ciphertext, and key bits==
  - **Padding Oracle Attacks**
    - ==Exploits incorrect padding in cryptographic systems to recover plaintext by sending carefully crafted ciphertexts==

## Quantum Cryptography
  - **Quantum Key Distribution (QKD)**
    - ==Uses quantum mechanics to ensure secure communication==
  - **Shor's Algorithm (Breaking RSA)**
    - ==Breaks RSA and ECC by efficiently factoring large numbers==
  - **Grover's Algorithm (Speeding up Symmetric Key Search)**

