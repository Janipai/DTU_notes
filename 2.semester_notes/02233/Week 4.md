### Exercise 1
1. We just used RSA with a key length of 1024. Can you see any potential issues already?
2. We created our CSR from a private key. What would happen if we shared this key?

1
**RSA keys** are mathematical objects with a lot of internal structure. The biggest integer whose value lies between $2^{1023}$ and $2^{1024}$. To break an RSA key, you "just" have to [factor](http://en.wikipedia.org/wiki/Integer_factorization) this modulus into its prime factors. 

With a small cluster of 81 Pentium 4 chips and 104 hours of processing time, they were able to successfully [hack](https://www.engadget.com/tag/hack/) 1024-bit encryption in OpenSSL on a SPARC-based system
https://www.engadget.com/intuitive-machines-moon-lander-sent-home-its-first-images-and-theyre-breathtaking-194208799.html?guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAAGUhg0ty8bad5pU5X_5WkHpTrLHDJQMw_OTPJesSm3w0eSVJcInYZd4dWoIdSkg9n-C3yIQSOuR45oLufJMehonjsX6ikrbRdzQ2BmSJhmgHSWuayzuQlzV1t9Ci9rQMDXUKOL47tPfLqainAwLDrLnrLrcVbYFmm_xgTPYAVS2r&guccounter=2
2
when creating the CSR with the same private key, it gives the exact same CSR. So anybody can use the CSR 

### Exercise 2
1. What would happen if we connected to a server with expired certificates? 
2. Can you see any potential issue with extending the validity of the certificate? 
3. What about connecting to a server with a certificate generated using weak cryptographic functions? 

1:
You will be unauthorized

2:
if you extend the validation, the security decreases, as it doesn generate new certificates, that checks if you are authorized.

3:
Vulnerably to attacks as bruce-force attacks, since it is using a weak cryptographic functions

### Exercise 3
The connection is not private

### Exercise 4
