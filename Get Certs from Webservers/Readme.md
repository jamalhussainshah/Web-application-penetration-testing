This lab is created by ghanimah in canada for education purpose in order to capture the flag. 

What is certificate handshake?
The SSL or TLS handshake enables the SSL or TLS client and server to establish the secret keys with which they communicate. This section provides a summary of the steps that enable the SSL or TLS client and server to communicate with each other. Agree on the version of the protocol to use.

Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the SSL Handshake.

Run the below command
openssl s_client -showcerts -servername domain -connect domain:443

# pentools
GetCertNames:

Takes targets (-t) in IP, FQDN, or CIDR format and combines them with ports (-p) and extracts the CN and the Subject Altrnate Names from the certificate. By default, the script will randomize the host and ports but it can be disabled with -r. The -v option can be used to show the verbose actions.


What is SSL Handshake ?

SSL Handshake

The communication over SSL always begins with the SSL handshake. The SSL handshake is an asymmetric cryptography which allows the browser to verify the web server, get the public key and establish a secure connection before the beginning of the actual data transfer.

The following figure illustrates the steps involved in the SSL handshake:
SSL Handshake

Let's understand the above steps:

The client sends a "client hello" message. This includes the client's SSL version number, cipher settings, session-specific data and other information that the server needs to communicate with the client using SSL.

The server responds with a "server hello" message. This includes the server's SSL version number, cipher settings, session-specific data, an SSL certificate with a public key and other information that the client needs to communicate with the server over SSL.

The client verifies the server's SSL certificate from CA (Certificate Authority) and authenticates the server. If the authentication fails, then the client refuses the SSL connection and throws an exception. If the authentication succeeds, then proceed to step 4.

The client creates a session key, encrypts it with the server's public key and sends it to the server. If the server has requested client authentication (mostly in server to server communication), then the client sends his own certificate to the server.

The server decrypts the session key with its private key and sends the acknowledgement to the client encrypted with the session key.

Thus, at the end of the SSL handshake, both the client and the server have a valid session key which they will use to encrypt or decrypt actual data. The public key and the private key will not be used any more after this. 

Regards
Jamal H. Shah
