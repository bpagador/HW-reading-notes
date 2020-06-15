#### Reading

* user modeling 
    * refers to the particular way in which user information is stored
    * the rule of thumb is that sensitive information needs to be encrypted
        * this protects the user's data from even developers with database permission
    * if your app requires that use be able to read other user's personal info, a second user model should be created that displays the necessary data and strictly limits access to the sensitive user info like passwords 

* cryptography
    * cooler hacker sh*t!
    * well, more specifically, the ability to decode secret information using a key
    * cryptography also has a branch called cryptanalysis: the science of decoding encrypted messages without a having the proper key

* hash algorithms
    * often used to check the integrity of data 
    * the hash is like the middleman between front end and server
        * when a password is entered, it gets encrypted by the hash algorithm which stores that password and produces a hash
        * this hash is how the server read the password entered on the front end to see if the hash data matches what was stored
        * if it does, you get authorized and log in!

* basic authorization
    * the kind of authorization that doesn't need or require hash encryption, it uses something called base64 encoding instead
    * a username and password is sent in an http request and get encoded into a string 
    * the resulting string is set to the value of the authorization header (remember postman, chea cheaaaa)
    * the server is then able to decode the basic auth header, read the user info, and return a token
    * use this token to re-authenticate yourself over and over again 
