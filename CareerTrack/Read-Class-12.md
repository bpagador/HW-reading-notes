#### Why you should use BCrypt to hash passwords?

* plain text password: the least safe, can be replicated across other logins, making the password susceptible to hackers

* one way hash: password has a hashing algorithm, still can get hacked into because the system is not exactly a one way system

* salting: adds a long string of bytes, so even if password gets accessed, the string does not--however, with access to your source code, can still get hacked 

* random salt for each user: user accounts, multiple salt encryptions, takes longer to hack into but still possible 

* the bcrypt solution:
    * slows down the hacking process until it is no longer a viable strategy
    * uses a Key Factor, a feature of the computer, which can adjust the cost of hashing (time)
    * hash output can be influenced with key factor changes (those numbers: 14, 8?)

#### Hashing in Action: Understanding bcrypt
* ideal authentication platform would integrate both hashing and salting
* cryptographic functions to choose from:
    * SHA2
    * SHA-3
* design problem: SHA families were designed to be computationally fast
* how fast a cryptographic function can calculate a hash === how safe the password is
    * faster calculations mean faster brute-force attacks
    * remember: a function that is slow at hashing passwords stops hacker in their tracks

* bcrypt:
    * combines the expensive key setup phase of the Blowfish cipher with a variable number of iterations to increase the workload and duration of hash calculations
        * this makes it scalable: iteration counts can be increased to slow down decryption as computer power grows


#### Token Storage

* tradition web app = store token server side on in a session cookie
    * cookie needs to be encrypted
* native/mobile app = store token in KeyStore of KeyChain and limit access to that storage
* single-page app scenario = recommendation is Auth0 SPA SDK which handles token storage, session management
* browser in-memory scenarios = store token in browser memory, using Web Workers or Javacript closures 