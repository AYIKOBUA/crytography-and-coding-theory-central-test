AYIKOBUA DAN

2023/U/MMU/BCS/01663


THE BRIEF DESCRIPTION OF THE IMPLEMENTATION:


a) RSA ENCRYPTION
A public-key encryption algorithm which is used as secure data transmission. 
RSA (Rivest–Shamir–Adleman) That includes the creation of a couple keys — one for encrypting and another key(which is private) to decrypt it.

Implementation Steps:

Key Generation:

Generate a new RSA key pair (public and private keys) of bits 2048 from the cryptography library that comes with Python.

Where the private key is for decryption, & public key is used for encryption.

Encryption:

Convert Message ("Hello, World!") into a byte format.

Encrypt the message with RSA public key

Decryption:

Decrypt the message (ciphertext -> original form) using your private key.



b) DIFFIE HELLMAN KEY EXCHANGE:
The Diffie-Hellman algorithm is a key exchange method which allows two parties to create a shared secret over an unsecured link. This key, on the other hand can be used with symmetric encryption.

Implementation Steps:

Key Exchange:

Where both Alice and Bob agree on a large prime number p, along with base 'g' (both are public).

Both parties independently of each other create their private key, and calculate the public value using g^private_key % p (power in diagram it is also lowercase letter c).

Both Alice and Bob calculate shared secret key using their own public values.

Encryption & Decryption:

You will use a symmetric encryption algorithm(e.g. AES) to encrypt and decrypt the message with teh shared secret key.



c) HASH FUNCTIONS (SHA-256):
SHA-256 (part of the SHA-2 family) is a cryptographic hash function that takes an input and produces a 256-bit hash value.

Implementation Steps:
Compute Hash:

Given a message, use Python’s hashlib to compute the SHA-256 hash of the message.
Verify Integrity:

To verify the message's integrity, recompute the hash of the received message and compare it with the original hash.



d) DIGITAL SIGNATURES:
ECDSA (Elliptic Curve Digital Signature Algorithm) is algorithm that is used for digital signatures. It involves generating a key pair and using the private key to sign a message. The public key is used to verify the signature.

Implementation Steps:
Key Pair Generation:

 You generate a private and public key using elliptic curve cryptography (ECC).
Sign a Message:

Use the private key to create a digital signature of the message.
Verify the Signature:

Verify the signature using the public key and ensure that the message matches the signature.
THE END 
