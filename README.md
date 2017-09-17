# security

#### Perfect Forward Secrecy(PFS)
PFS is achieved by using random(Ephemeral) value as private key of DH/ECDH key exchange algorithm for each SSL connection. The shared secret key of DH/ECDH is used to derived AES encryption/decryption key during data exchange. With DHE/ECDHE, RSA is only used for authentiaion, not for key encryption. <br>
PFS ensures that even if all the traffic is recorded and the server's private key is comprised in the future, the history record still can not be recovered(decrypted), except that all the ephemeral values were recorded.


https://vincent.bernat.im/en/blog/2011-ssl-perfect-forward-secrecy

#### how does SSH work?
https://www.ucolick.org/~sla/ssh/ssh.howto.html
