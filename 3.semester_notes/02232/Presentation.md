**State of the art**
We had a look at three different existing solutions on password store managers.
Some of the major different on them are that Nordpass that are using XChaCha20 as a symmetric encryption algorithm.
The key different is that AES breaks data into block and encrypt each of them, while XChaCha20 encrypt each bit. AES do also often requires special hardware to run efficiently, whereas XChaCha20 works well on regular software.

Another difference between these existing solutions is that Bitwarden is using PBKDF and Argon2id, while 1Password is only using PBKDF and NordPass is only using Argon2id.

KDFs is used to hash passwords. PBKDF2 has some weakness and one of them is its vulnerability to GPU-based attacks. 
Argon2id is a hybrid of Argon2i and Argon2d, which means it is faster and is designed to be resistant to side channel attacks and to time-memory trade-off attacks. 

Argon2id is also highly customizable, allowing adjustment of different parameters.



Bitwarden is the only one that is open source, and  we noticed that their white paper is more well documented.

**Login**
Under the login process, the user enter their email and password, that will be hashed with a Argon2id to a master key. This master key will again be hashed with a salt from the entered password  and that hash will be compared with the hash on the server, that was stored from the sign up phase. 
We have also added an optional multi factor authentication for adding an extra layer of security. 

**New slide**
If the comparison is correct, the server will get the protected symmetric key and the encrypted vault data. These are both encrypted with AES-256 and will be decrypted locally on the users device 
