#### Kerckhoffs’ principle
[The method] must not be required to be secret, and it must be able to fall into the enemy’s hands without causing inconvenience.
all of the security of the system should be concentrated in the secrecy of the key, not the secrecy of the algorithms


Encryption scheme:
- Enc
- Dec
- KeyGen

one-time pad (OTP)
We generally use the variable λ to refer to the length (# of bits) of the secret key in a scheme
(λ = 10 is “just as secure” as λ = 1000)
λ is often called the security parameter of the scheme

