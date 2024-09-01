Cryptography I
Cryptography solve problems:

- keeping secrets
    - messages on network
    - data stored on disk, memory cards, USB sticks
- ensuring integrity
    - messages on network (message authentication codes)
    - data stored on disk
- authentication
    - user authentication
    - message authentication

Keeping secrets

- steganography
    - hide the existence of a secret message
    - if the message is found, then the secret is revealed
- codes
    - ww 2 gave code about the war by talking about something else, like the weater
    - you dont know if there is a hidden message
- ciphers
    - scramblin according to an agreed algorithm

Secret writing

- steganography (hidden)
- cryptography (scrambled)
    - subsitution
        - code
        - cipher
    - transposition
        - Ciphe

bacis building blocks of cryptography

- symmetric
- asymmetric
- hash function
- digital signatures
    - private key
    - public key
- advanced algorithms, protocols and constructs not covered here

Message Authentication codes (MAC)

- message authentication codes protect integrity of messages
- hash-based mac uses a cryptographic hash function and a shared secret

security properties

- sym
    - confidentiality of messages
    - both parties know the shared key
- asym
    - confidentiality of messages
    - only one party know the secret key
- hash func
    - hash value corresponds to given M
- MAC
    - Integrity and authenticity
    - non-repudiation of message
- Digital signatures

3 classes of attacks on crypto-systems

- attacking the cipher (we can guess it, if it is a small number)
- attacking the key
- attacking the cryptographic

ECB reflects plaintext

limitation

it is not used to large amount of data

---

more
![[Pasted image 20240831125052.png]]