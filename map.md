---
title: Cryptography Mindmap
markmap:
  colorFreezeLevel: 5
---

## Classical Cryptography

### <span title="Rearranges the letters or groups of letters in a message without changing them">**Permutation Ciphers**</span>   
  
  - <span title="Arranges text in a zigzag pattern on multiple lines and then reads it row by row.">Rail Fence Cipher</span>   
  
  - <span title="Writes the message in rows and reads it in columns according to a keyword.">Columnar Transposition Cipher</span>
  
### <span title="Replaces each letter in the plaintext with another letter, often according to a fixed system">**Substitution Ciphers**</span>   
  
  - <span title="Shifts each letter by a fixed number in the alphabet">Caesar Cipher</span> 

  - <span title="Uses a keyword to determine shifts for each letter, making it harder to break.">Vigenère Cipher</span>

  - <span title="Reverses the alphabet (A = Z, B = Y, etc.).">Atbash Cipher</span>
  
  - <span title="Uses a 5x5 grid of letters and digraphs to encrypt.">Playfair Cipher</span>

  - <span title="Encrypts letters in blocks using matrix multiplication with a key matrix.">Hill Cipher</span>
  
### <span title="A type of substitution cipher that uses multiple substitution alphabets to encrypt the message. It changes the substitution system at different points in the text, making it more resistant to frequency analysis">**Polyalphabetic Ciphers**</span>    

  - <span title="Uses a keyword to determine shifts for each letter, applying a different substitution alphabet at each position">Vigenère Cipher</span>
  - <span title="Similar to the Vigenère Cipher but uses subtraction in place of addition during encryption.">Beaufort Cipher</span>
  
  - <span title="A method used to crack substitution ciphers by analyzing how frequently certain letters appear in the ciphertext and comparing these frequencies to typical letter distributions in the language. For example, in English, E is the most common letter. If the most frequent letter in the ciphertext is Q, it might correspond to E in the plaintext.">Frequency Analysis Techniques</span>  


## Modern Cryptography

###  <span title="Algorithms that use the same cryptographic keys for both the encryption of plaintext and the decryption of ciphertext.">**Symmetric Cryptography**</span> 
 
  - <span title="Encrypts data one bit or byte at a time.">Stream Ciphers</span> 
    - ChaCha20
    - Salsa20
    - RC4
  - <span title="Encrypts data in fixed-size blocks (e.g., 64 or 128 bits).">Block Ciphers</span> 
    - DES
    - 3DES
    - AES
    - Blowfish
    - Twofish
  - <span title="Techniques to securely encrypt large amounts of data">Modes of Operation</span> 
    - ECB (Electronic Codebook)
    - CBC (Cipher Block Chaining)
    - CFB (Cipher Feedback)
    - OFB (Output Feedback)
    - CTR (Counter Mode)

### <span title="Cryptographic algorithms that use a pair of related keys (one public key and one private key).">**Asymmetric Cryptography**</span> 
 
  - <span title=" process that uses public key to encrypt and related private key to decrypt a message">Encryption</span> 
    - <span title="Relies on the difficulty of factoring large numbers">RSA (Rivest–Shamir–Adleman)</span> 
    - ElGamal
    - <span title="It's based on algebraic structures of elliptic curves over finite fields">ECC (Elliptic-Curve Cryptography)</span> 
      - Curve25519
      - P-256

  - <span title="Use for secure key exchange over an insecure channel">Key Exchange</span> 
    - Diffie–Hellman (DH)
    - Elliptic-Curve DH (ECDH)

  - <span title="Verify the authenticity of digital messages or documents">Signature</span>
    - DSA
    - ECDSA
    - Schnorr 


## Post-quantum Cryptography

### **Lattice-based**
  - Key Encapsulation
    - NTRU
    - Kyber
    - FrodoKEM
  - Signature
    - Dilithium
    - Falcon
### <span title="PQC cryptosystems whose security depends, in part or entirely, on the difficulty of decoding a linear error-correcting code"> **Code-based** </span> 

  - Key Encapsulation
    - Classic McEliece
    - Bike
  - Signature
    - Niederreiter

###  <span title="PQC Signature algorithms whose security is mathematically based on the security of a selected hash function">**Hash-based Signatures**</span> 
  - XMSS
  - Sphincs+

### <span title="PQC cryptographic primitives based on multivariate polynomials over a finite field F">**Multivariate-based** </span> 

  - Key Encapsulation
    - Matsumoto-Imai
    - HFE
  - Signature
    - Matsumoto-Imai
    - Rainbow

###  <span title="It utilizes a rational map between elliptic curves (isogenies) to provide post-quantum secure cryptographic primitives">**Isogeny-based**</span> 
  
  - Sike


##  <span title="They Can be used to map data of arbitrary size to fixed-size values">Hash Functions</span>
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
  - Certificates Authorities (CA)
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

## Cryptography Threats
  -  <span title="Tries every possible key until the correct one is found">**Brute Force Attack**</span>

  -  <span title="Analyzes the frequency of letters or groups of letters to crack substitution ciphers">**Frequency Analysis (Classical Ciphers)**</span>
  
  - <span title="The attacker has access to both the plaintext and its corresponding ciphertext and uses this information to derive the key">**Known-plaintext Attack**</span>

  - <span title="The attacker can choose arbitrary plaintexts and obtain their corresponding ciphertexts, allowing them to gather information to break the encryption">**Chosen-plaintext Attack**</span>
  
  - <span title="The attacker can decrypt chosen ciphertexts and use this to gain information about the encryption key or algorithm">**Chosen-ciphertext Attack**</span>

  -  <span title="A known-plaintext attack that targets block ciphers by using a space-time tradeoff, working faster than brute force by exploiting the structure of two-key encryption schemes">**Meet-in-the-Middle Attack**</span>

  - <span title="Exploits physical leakages like timing or power consumption to break encryption">**Side-Channel Attacks**</span>
    -  <span title="Measures the time it takes to perform cryptographic operations to deduce secret keys">Timing Attacks</span>

    - <span title="Monitors power consumption during encryption to extract information about the key">Power Analysis</span>

  - <span title="Analyzes the differences in ciphertexts resulting from slight differences in the plaintext to discover the secret key"> **Differential Cryptanalysis**</span>

  - <span title="Uses linear approximations to describe the behavior of block ciphers and analyzes the relationships between plaintext, ciphertext, and key bits">**Linear Cryptanalysis**</span>

  - <span title="Exploits incorrect padding in cryptographic systems to recover plaintext by sending carefully crafted ciphertexts">**Padding Oracle Attacks**</span>

  - <span title="Use quantum computer to break the existing cryptography algorithms">**Quantum computing**</span>
    - <span title="Breaks RSA by efficiently factoring large numbers and ECC by discrete logarithm">Shor's Algorithm </span>
    - <span title="Speeding up Symmetric Key Search">Grover's Algorithm </span>

## Misc Algorithms
  - <span title="a form of encryption with an additional evaluation capability for computing over encrypted data without access to the secret key"> **Homomorphic Encrypton** </span> 
  - <span title="Methods for distributing a secret among a group, in such a way that no individual holds any intelligible information about the secret, but when a sufficient number of individuals combine their 'shares', the secret may be reconstructed"> **Secret Sharing** </span>  
  - <span title="a shift register whose input bit is a linear function of its previous state."> **Linear Feedback Shift Register (LFSR)** </span>   



