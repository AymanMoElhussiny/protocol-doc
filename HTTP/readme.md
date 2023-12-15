## I am tring to explain more about HTTP and HTTPS protocols as these are part of most important protocls that we are dealing with 

## HTTP 
### What is HTTP? 
An HTTP stands for Hypertext Transfer Protocol. The HTTP protocol provides communication between different communication systems. When the user makes an HTTP request on the browser, then the webserver sends the requested data to the user in the form of web pages. In short, we can say that the HTTP protocol allows us to transfer the data from the server to the client.

An HTTP is an application layer protocol that comes above the [TCP layer](https://github.com/AymanMoElhussiny/protocol-doc/blob/07446800c04923c8a1644b632145d204329659c9/TCP/README.md). It has provided some standard rules to the web browsers and servers, which they can use to communicate with each other.

An HTTP is a stateless protocol as each transaction is executed separately without having any knowledge of the previous transactions, which means that once the transaction is completed between the web browser and the server, the connection gets lost.


### What is HTTPS?
The full form of HTTPS is Hypertext Transfer Protocol Secure. The HTTP protocol does not provide the security of the data, while HTTP ensures the security of the data. Therefore, we can say that HTTPS is a secure version of the HTTP protocol. This protocol allows transferring the data in an encrypted form. The use of HTTPS protocol is mainly required where we need to enter the bank account details. The HTTPS protocol is mainly used where we require to enter the login credentials. In modern browsers such as chrome, both the protocols, i.e., HTTP and HTTPS, are marked differently. To provide encryption, HTTPS uses an encryption protocol known as Transport Layer Security, and officially, it is referred to as a Secure Sockets Layer (SSL). This protocol uses a mechanism known as asymmetric public key infrastructure, and it uses two different keys which are given below:

Private key: This key is available on the web server, which is managed by the owner of a website.
It decrypts the information which is encrypted by the public key.
Public key: This key is available to everyone. It converts the data into an encrypted form

Here's a comparison table between HTTP (Hypertext Transfer Protocol) and HTTPS (Hypertext Transfer Protocol Secure):

| Feature                            | HTTP                                | HTTPS                                               |
|------------------------------------|-------------------------------------|-----------------------------------------------------|
| **Security**                       | Not secure                          | Secure (data is encrypted during transmission)      |
| **Encryption**                     | No encryption                       | Uses [SSL/TLS](SSL-TLS.md) encryption for secure data transfer    |
| **URL Scheme**                     | Begins with "http://"                | Begins with "https://"                               |
| **Default Port**                   | 80                                  | 443                                                 |
| **Data Integrity**                 | No guarantee                        | Ensures data integrity during transmission          |
| **Confidentiality**                 | No confidentiality                  | Ensures data confidentiality through encryption     |
| **Authentication**                 | No authentication                   | Provides authentication through SSL/TLS certificates|
| **Browser Indicators**              | No padlock or "Secure" label        | Displays padlock symbol and "Secure" label in the address bar |
| **Search Engine Ranking**           | May not contribute positively      | Contributes positively to search engine ranking      |
| **Usage**                          | Suitable for non-sensitive data    | Essential for transmitting sensitive information     |
| **Examples of Use**                 | News websites, general content      | Online banking, e-commerce, login pages, forms        |
| **Performance Impact**              | Generally faster                    | Slightly slower due to the overhead of encryption   |
| **Common Risks**                    | Man-in-the-middle attacks, data interception | Eavesdropping, unauthorized access to sensitive data |

**Note:** While HTTP and HTTPS represent two ends of the security spectrum, it's important to note that the move towards securing websites is increasingly prevalent, and many websites now default to HTTPS to ensure a secure and private user experience. The adoption of HTTPS is particularly crucial for websites handling sensitive information, such as login credentials, personal details, and financial transactions.

Refrences:
- [HTTP vs HTTPS](https://www.javatpoint.com/http-vs-https)
