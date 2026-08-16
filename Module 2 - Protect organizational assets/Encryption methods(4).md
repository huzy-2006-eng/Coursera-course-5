### CRYPTOGRAPHY -
The process of transforming information into a form that unintended readers can't understand.

#### Algorithm - 
A set of rules used that solve a problem.

#### Cipher - 
An algorithm that encrypts information.

#### Cryptograhic key -
A mechanism that decrypts ciohertext.

#### Brute force attack -
A trial and error process of discovering private information.

#### Public key infrastructure (PKI) - 
An encryption framework that secures the exchange of information online.

## Public key infrastructure process- 
1. Exchange of encrypted information:
This involves either asymmetric encryption or symmetric encyrption or both.
   Asymmetric encryption - The use of a public and private key pair for encryption and decryption of data.
   The private key is only given to users with authorized access.

   Symmetric enryption - The use of single secret key to exchange information.
   ecause it uses one key for encryption and decryption, the sender and receiver must know the secret key to lock or unlock the cipher.

2.  Eslablish trust using a system of digital certificates:
Digital certificate - A file that verifies the identity of a public key holder.

### Note - One drawback to having long encryption keys is slower processing times. Although short key lengths are generally less secure, they’re much faster to compute. Providing fast data communication online while keeping information safe is a delicate balancing act. 


#  Symmetric algorithms:
1. Triple DES (3DES) is known as a block cipher because of the way it converts plaintext into ciphertext in “blocks.” Its origins trace back to the Data Encryption Standard (DES), which was developed in the early 1970s.

2. DES was one of the most earliest symmetric algorithms that generated 64 bit keys,  although only 56 bits are used for encryption.

3.  A bit is the smallest unit of data measurement on a computer. 

4. Triple DES applies DES algorithm 3 times, using three different 56 bit keys.

5. key length = 168 bits.

6. AES(ADVANCED ENCRYPTION STANDARD) is one of the most secure symmetric algortihms today.

7. AES generates keys of 128,192,256 bits.
 Cryptographic keys of this size are considered to be safe from brute force attacks. It’s estimated that brute forcing an AES 128-bit key could take a modern computer billions of years!

# Asymmetric algorithms:
1. Rivest Shamir Adleman (RSA) is named after its three creators who developed it while at the Massachusetts Institute of Technology (MIT).

2. RSA is one of the first asymmetric encryption algorithms that produces a public and private key pair.

3. Asymmetric algorithms like RSA produce even longer key lengths. In part, this is due to the fact that these functions are creating two keys. RSA key sizes are 1,024, 2,048, or 4,096 bits. RSA is mainly used to protect highly sensitive data.

4. Digital Signature Algorithm (DSA) is a standard asymmetric algorithm that was introduced by NIST in the early 1990s. DSA also generates key lengths of 2,048 bits. This algorithm is widely used today as a complement to RSA in public key infrastructure.

# Generatiing keys:
1. These algorithms must be implemented whenn an organization chooses one to protect their data. One way this is done is using OpenSSL.

2. OpenSSL is an open-source command-line tool that can be used to generate public and private keys.

3. OpenSSL is commonly used by computers to verify digital certificates that are exchanged as part of public key infrastructure.

4. In early 2014, OpenSSL disclosed a vulnerability, known as the Heartbleed bug, that exposed sensitive data in the memory of websites and applications. Although unpatched versions of OpenSSL are still available, the Heartbleed bug was patched later that year (2014). 

# Obscurity is not security:
1. In the world of cryptography, a cipher must be prove to be unnbreakable  before claiming that it is secure.

2. According to Kerckhoff's principle, cryptography should be designed in such a way that all the details of an algorithm--except for the private key--should be knowable without sacrificing its security.

3. For example, you can access all the details about how AES encryption works online and yet it is still unbreakable.

# Encryption is everywhere:
1. For example, websites tend to use asymmetric encryption to secure small blocks of data that are important.
Usernames and passwords are often secured with asymmetric encryption while processing login requests.
Once a user gains access, the rest of their web session often switches to using symmetric encryption for its speed.

2. Using data encryption like this is increasingly required by law. Regulations like the Federal Information Processing Standards (FIPS 140-3) and the General Data Protection Regulation (GDPR) outline how data should be collected, used, and handled. Achieving compliance with either regulation is critical to demonstrating to business partners and governments that customer data is handled responsibly.

# COMMMANDS:
 For Decrypting CAESAR CIPHER - 
 1. cat .<filename> | tr "d-za-cD-ZA-C" "a-zA"
 The tr command translates text from one set of characters to another, using a mapping. The first parameter to the tr command represents the input set of characters, and the second represents the output set of characters. Hence, if you provide parameters “abcd” and “pqrs”, and the input string to the tr command is “ac”, the output string will be “pr".

 In this case, the command tr "d-za-cD-ZA-C" "a-zA-Z" translates all the lowercase and uppercase letters in the alphabet back to their original position. The first character set, indicated by "d-za-cD-ZA-C", is translated to the second character set, which is "a-zA-Z".

2. openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute

In this instance, the openssl command reverses the encryption of the file with a secure symmetric cipher, as indicated by AES-256-CBC. The -pbkdf2 option is used to add extra security to the key, and -a indicates the desired encoding for the output. The -d indicates decrypting, while -in specifies the input file and -out specifies the output file. The -k specifies the password, 
which in this example is ettubrute.

# Non repudiation and Hasing: 
Hash function - An algorithm that produces a code that can't be decrypted.

Non-repudiation - The concept that the authenticity of information can't be denied.

{Hashing is widely used for authentication and non-repudiation}

One of the earliest hash functions is Message Digest 5(MD5).
(Professor Ronald Rivest)

# Hash Collisions:
1. One of the flaws in MD5 happens to be a characteristic of all hash functions.
2.  Hash algorithms map any input, regardless of its length, into a fixed-size value of letters and numbers.
3. what's the problem with that? Although there are an infinite amount of possible inputs, there’s only a finite set of available outputs!
4. MD5 values are limited to 32 characters in length. Due to the limited output size, the algorithm  is considered to be vulnerable to hash collision, an instance where different inputs generate the same hash value.
5. Because hashes are used for authentication,a hash collision is similar to copying someone's identity.
6. Attackers can carry out collision attacks to fraudulently impersonate authentic data.

# Next-generation hashing:
1. To avoid the risk of hash collisions,functions that generated longer values were needed. MD5's shortcomings gave way to a new group of functions known as the Secure Hashing Algorithms, or SHAs.

2. The National Institute of Standards and Technology (NIST) approves each of these algorithms. Numbers besides each SHA function indicate the size of its hash value in bits. Except for SHA-1, which produces a 160-bit digest, these algorithms are considered to be collision-resistant. However, that doesn’t make them invulnerable to other exploits.

Five functions:
A. SHA-1
B. SHA-224
C. SHA-256
D. SHA-384
E. SHA-512


# Secure password storage:
1. Passwords are typically stored in a database where they are mapped to a username. The server receives a request for authentication that contains the credentials supplied by the user. It then looks up the username in the database and compares it with the password that was provided and verifies that it matches before granting them access.

2. This is a safe system unless an attacker gains access to the user database. If passwords are stored in plaintext, then an attacker can steal that information and use it to access company resources. Hashing adds an additional layer of security. Because hash values can't be reversed, an attacker would not be able to steal someone's login credentials if they managed to gain access to the database.

# Rainbow tables:
A rainbow table is a file of pre-generated hash values and their associated plaintext. They're like dictionaries of weak passwords. Attackers capable of obtaining an ogranization's password database can use a rainbow table to compare them against all possible values.

# Adding some "salt":
1. Salting is an additional safeguard that's used to strenghten hash functions.
2. A salt is a random string of characters that's added to data before it's hashed.
3. The additional characters produce a more unique hash value, making salted data resilient to rainbow table attacks.
4. For example, a database containing passwords might have several hashed entries for the password "password." If those passwords were all salted, each entry would be completely different. That means an attacker using a rainbow table would be unable to find matching values for "password" in the database.
5. The length and uniqueness of a salt is important. Similar to hash values, the longer and more complex a salt is, the harder it is to crack.

#### COMMAND TO GENERATE HASH VALUE OF A FILE:
1. sha256sum <filename.txt>

2. sha256sum file1.txt >> file1hash
(file1hash is a new file which contains the output)
(file1.txt is the file from which we generated a hash value)

