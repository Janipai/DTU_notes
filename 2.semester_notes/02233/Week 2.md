### Exercise 1
(**Unconditional Security**) During the lecture you have learned that encryption algorithms can be broken if one can guess the secret key. There exists a symmetric key encryption scheme for which this is not the case - i.e., which is secure against such attacks. This is usually called the One-Time Pad. It is defined as follows: 

**Key Generation** To generate the key k, flip a fair coin. If it is heads, then set k = 0, else set k = 1. 
**Encryption** Encrypt the message bit m as follows: compute c = m + k mod 2 and output c. **Decryption** Decrypt the ciphertext bit c as follows: compute m′ = c + k mod 2 and output m′ 

1. Show that this scheme actually decrypts to the right plaintext. 
$$
K = \{0,1\}^\lambda
$$
$KeyGen():$
$$Output\: k \leftarrow K $$
$Enc(k,m \in M):$
$$
Output\: Enc(m)
$$
The cipher text is defined to be
$$
c=Enc(m)=m+k\: mod\: 2
$$$Dec(k,c \in C):$
$$
Output\: k^{-1}(c)
$$
The plain text is the inverse of the $Dec(k,c)$
$$
m'=Dec(c)=c+k\: mod\: 2=(m+k\:mod\:2)+k\:mod \:2
$$
We have now proved that $m'=m$


2. What can go wrong if you use the same key for two encryptions? 
An attacker might know what the key is based on it is a one time pad scheme. This is due to OTP reused the key, so it's very secure if we only use the algorithm once.

3. Can you use this scheme to also encrypt a long string of bits? How do you have to modify it? What is the disadvantage of this encryption scheme, in terms of practicality?
It can either be modified to use block ciphers that convert a block of bits to a cipher text. In practicality this wont be efficient, due to the pattern when making the the key to have the same length of the plain text.
That is why we use counter mode

### Exercise 2

(AES) Assume you obtain the ciphertext

U2F sdGV kX1 + EqkW b5RzDhZyL6gSu/2hCuW RF kBF aO2U =

You know that it is an AES-128 ECB encryption of an UTF-8-encoded text that starts with the four characters “HELP”. The ciphertext is encoded in Base-64.

1. Assuming that you have no further information about the key, why can you not simply run a brute-force attack to recover the rest of the message?
We don't have enough information to compute the rest of the key.

2. Assume that you have additionally learned that the key has the first 96 bits set to 0. Why is an attack now plausiblea ? 
We know 96 out of 128 bits, which make i computational possible to calculate the rest of the key.

3. Assume that you learn that only 4 bits of the key are set to 1, while the remaining ones are set to 0. Does this mean that an attack is feasible? 

k is the number of known bits in the key (4 bit)
n is the key  that is 128 bit long

due to the binomial coefficient, we calculate
$$n!/{k!\cdot(128-4)!}=10668000$$
and all possible combination of k is
$$2^{128}=3.4028237e+38$$
this is way harder to compute than the 1068000

4. The ciphertext is not given as a string, but encoded in Base64. Investigate what Base64 is. Why can it be advantageous to encode a ciphertext in Base64 instead of sending it directly over the channel? 
It is harder to read a base64 format than the ciphertext and base64 formattet is only 6 bit while ciphertext is 8 bit long.

5. The message mentioned in this exercise has been encrypted using the openssl tool available on any Linux system. Assume that the key has been derived from “crypto” (using the −k option). Attempt to decrypt it!
echo -n "U2F sdGV kX1 + EqkW b5RzDhZyL6gSu/2hCuW RF kBF aO2U =" | openssl enc -d -aes-128-ecb -k crypto

bad magic number

### Exercise 3
It is computation to compute all phone numbers
$10⁸=100000000$

All these numbers is hashed in the server.
if a Rainbow attack is done on the server.