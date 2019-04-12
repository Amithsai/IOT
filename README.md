# Cryptography for Iot devices

Security is a major concern in IOT devices sice the day it came into action this project focuses on encrypting the message so that it cannot be accessed by ohter who do not have the right key.

This example is an implementation of Socket Programming with addition of SSL and AES implementations using Python. 

Requirements for this implementation are a private key and a server certificate generated using the private key, both of which can be generated using openssl.

The inner layer is of AES encryption. The data to be sent is encrypted and decrypted using AES objects.

The outer layer is of SSL. The method ssl.wrap_socket() will wrap the socket with the required security considerations. In this example, only a key and a self signed certificate have been provided to ssl.wrap_socket(), and the other options have been left which are automatically set as default. This is however not recommended in Python documentation and the other options should be configured for better security.

We could use this model as a plugin to other IOT devices to send data securely through the internet.

### References:-

YOUTUBE LINK: 
