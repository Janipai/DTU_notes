xDescribe an attack that allows you to learn the length of a message that, say, Alice sends to Bob.
CBC has parallelized decryption algorithm
In CBC mode, the plaintext inuences the inputs to the block cipher, so these calls cannot be pre-computed before the plaintext is known.


In CBC mode, a plaintext consisting of ` blocks is encrypted into a ciphertext of ` + 1 blocks. In other words, the ciphertext leaks the number of blocks in the plaintext. We can leverage this observation into the following attack:
![[Pasted image 20240226093217.png]]

The distinguisher chooses a 1-block plaintext and a 2-block plaintext. If this distinguisher is linked to Lcpa-L, the 1-block plaintext is encrypted and the resulting ciphertext is 2 blocks (2λ bits) long. If the distinguisher is linked to Lcpa-R, the 2-block plaintext is encrypted and the resulting ciphertext is 3 blocks (3λ bits) long. By simply checking the length of the ciphertext, this distinguisher can tell the dierence and achieve advantage 1