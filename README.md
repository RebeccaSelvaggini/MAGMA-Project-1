# MAGMA-Project-1
Progetto per il corso di Algebraic Cryptography
Implementazione in linguaggio MAGMA di ELEPHANT Authenticated Encryption with Associated Data scheme (AEAD) nelle versioni Dumbo e Jumbo.
Implementazione del cifrario a chiave simmetrica “Elephant”:  
Authenticated Encryption with Associated Data (AEAD) scheme con costruzione nonce-based encrypt-then-MAC (Message Authentication Code)  
nelle versioni “Dumbo” e  “Jumbo” (algoritmo finalista nella competizione NIST LightWeight Cryptography).

Il codice è stato implementato in collaborazione con un altro studente utilizzando la documentazione ufficiale dei protocolli e date le seguenti richieste:

Your code has to contain four functions:

• Dumbo(K,N,A,M) for encrypting with Dumbo,
• Jumbo(K,N,A,M) for encrypting with Jumbo,
• DumboDec(K,N,C,A,T) for decrypting with Dumbo,
• JumboDec(K,N,C,A,T) for decrypting with Jumbo,

with the following specifications:

NAME: Dumbo(K,N,A,M)/Jumbo(K,N,A,M)
INPUTS: -K is the key as a sequence of 128 bits seen as a string of 32 hexadecimal digits,
        -N is the nonce as a sequence of 96 bits seen as a string of 24 hexadecimal digits,
        -A is the associated data as a sequence of arbitrary length seen as a string of hexadecimal digits,
        -M is the plaintext as a sequence of arbitrary length seen as a string of hexadecimal digits;
OUTPUT: -C is the ciphertext as a sequence of the same length as P as a string of hexadecimal digits,
        -T is the tag as a sequence of 64 bits seen as a string of 16 hexadecimal digits.

NAME: DumboDec(K,N,C,A,T)/JumboDec(K,N,C,A,T)
INPUTS: -K is the key as a sequence of 128 bits seen as a string of 32 hexadecimal digits,
        -N is the nonce as a sequence of 96 bits seen as a string of 24 hexadecimal digits,
        -C is the ciphertext as a sequence of arbitrary length seen as a string of hexadecimal digits,
        -A is the associated data as a sequence of arbitrary length seen as a string of hexadecimal digits,
        -T is the tag as a sequence of 64 bits seen as a string of 16 hexadecimal digits;
OUTPUT: -M is the plaintext as a sequence of arbitrary length seen as a string of hexadecimal digits.
