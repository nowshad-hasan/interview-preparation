- **Authentication VS Authorization**
  - Authentication tells us *Who are you*, like login to the application with username and password. But Authorization tells us about *What is user is permitted to do*. It can be managed with Role.

- **Encoding Vs Encryption Vs Hashing**
  - Encoding - It is a technique to transform data from one format to another. Few techniques are - Unicode, Base64, URL encoding, JWT. JWT is also Base64-URL, a variant of Base64 encoding combined with URL encoding. It has not security purpose and obviously it is a reversible process.
  - Encryption - It is a technique that makes the data unreadable, and hard to decode for an unauthorised user. It is for security so that attackers cannot attack in the middle. The main goal is data-confidentiality, protecting data from being accessed by unauthorised parties. Like encoding, it is also reversible process only for authorised people with `decryption key`. So, the challenge is to make this decryption process as hard as possible for unauthorised people. So, we must keep the key secret and change frequently. Two kind of key-based encryption algorithms exist. 
    - Symmetric-key algorithms: The algorithms used the same key to encrypt and decrypt data. Advanced Encryption Standard (AES) is an example of this family's algorithms.
    - Asymmetric-key algorithms - These algorithms use different keys to encrypt and decrypt data. RSA is an example.
  -Hashing - It is a technique where specific input always generates unique fixed-length string. Any small changes to the input will generate new hash. So, it ensures data integrity. And it is non-reversible process. Like - we store hash from user's password and then we compare if that is the same hash. But let's say we need to compare if user's uploaded image is already stored. So, we can compare the huge base64 data to our huge database's column. It will be an expensive operation. But what we can do, we can generate single hash from the picture, store it in the db - which is a fixed length string and then next time any uploaded image's hash can be compared with this. MD5 was a famous hashing algorithm but it is deprecated due to collision. SHA-256 is a modern algorithm.
    
  - Resources - [auth0](https://auth0.com/blog/encoding-encryption-hashing/)

- **What is Principal, Authentication Manager, Security Context, Granted Authority and Role?**
  -*Principal* -> When a user logged in into the system, their information like - username, userid or unique identifier is stored in the security context. It is called the principal.
  - *Authentication Manager* -> It is responsible to authenticate the user based on their credentials.
  - *SecurityContext* ->  After successful authentication, important information about logged in user and other details are stored in security context. It is available throughout the application. 
  - *Granted authority* -> Fine-grained authorization, we mean individual privilege, like - READ_PRIVILEGE, READ_AUTHORITY, CAN_EXECUTE_AS_ROOT. And we can restrict resource with this expression, *hasAuthority('READ_AUTHORITY')*.
  - *Role* -> It is coarse-grained authorization, where if any user has ADMIN role, he can access the resource. In spring security, it is a string prefixed with *ROLE*. We can restrict an user with *hasRole('ADMIN')*. Role is like a container of authorities/privileges. 

- **Coarse-Grained vs. Fine-Grained Authorization** 
  - Fine-Grained Authorization - It is more precise control over who can access which resource under particular conditions. It is complex to setup and manage as it has numerous specific policies and attributes. It supports least privilege and reduces security risks. It has use cases - 
    - Large enterprise - Complex structures requiring access controls to accommodate various roles, responsibilities and data sensitivity levels. 
    - Healthcare, finance systems, where strict compliance requirements and precise access controls required to protect sensitive information.
    - dynamic environments - access needs to adapt based on context, such as - user location, time,  device ensuring security in varying conditions.
  - Coarse grained authorization - It is access based on users or groups, like - all manager has the access to this resource. It is very simple to implement but cannot handle complex scenarios and potentially leading to over-permissioning. It is very suitable where straight forward access requirements. It has use cases - 
    - Small organisations - Limited resource and straightforward access needs. 
    - Low-sensitivity environments - where data and resources are not highly sensitive and risk is minimal.  
  - Resource - [Link](https://rublon.com/blog/coarse-vs-fine-grained-authorization/)

- **Please explain some basic terminology**
  - Authentication: Filters like UsernamePasswordAuthenticationFilter will extract username/ password from HTTP request & prepare Authentication type object
  - AuthenticationManager: Once received request from filter, it delegates the validating of the user details to the authentication providers available. Since there can be multiple providers inside an app, it is the responsibility of the AuthenticationManager to manage all the authentication providers available.
  - AuthenticationProvider: AuthenticationProviders has all the core logic of validating user details for authentication
  - UserDetailsManager/UserDetailsService : It helps in retrieving, creating, updating, deleting the User Details from the DB/storage systems.
  - PasswordEncoder: Service interface that helps in encoding & hashing passwords. Otherwise we may have to live with plain text passwords.
  - SecurityContext: Once the request has been authenticated, the Authentication will usually be stored in a thread-local SecurityContext  managed by the SecurityContextHolder. This helps during the upcoming requests from the same user. And it is available application wide.

- **What is CSRF and CSRF Token and how it is handled in Spring Security?**
  - CSRF stands for Cross Site Request Forgery. And to protect this, when we add spring-security library in our spring boot application, in the default login page, there is always *CSRF_TOKEN* added for the request of POST, UPDATE, DELETE http methods. It is because so that no attacker can send any post request without the token. The token is checked and validated by spring security itself. Yes, we can override the mechanism. So, we can say CSRF protection is enabled by default in spring security. So, this token is must for http MVC view based application where session is managed by cookie. The point is if the other site make the request (CORS is enabled in the server) on behalf of the actual user, the request is still valid. And it is authenticated as well because whichever site makes the request, cookies are sent everytime to the server. So, server cannot figure out that this request is malicious. For CORS enabling, response will not be fetched, but the request can be done, and it can devastate the database already. But what about JSON based application, where session is managed by JWT? We don't need that and that's why we disabled it in the security config.
  - Resources - [Baeldung](https://www.baeldung.com/spring-security-csrf), [Computerphile](https://www.youtube.com/watch?v=vRBihr41JTo&t=142s&ab_channel=Computerphile), Telusko](https://www.youtube.com/watch?v=8QDORHQvdu8&ab_channel=Telusko)

- **What is CORS?**
  - CORS stands for Cross Origin Resource Sharing. It is a browser feature where HTTP request can only be send from the same origin/domain or the allowed domain. It is a very powerful feature so that CSRF can not be done.

- **What is XSS?**
  - XSS stands for Cross Site Scripting. Let's say I want to hijack someone's cookie aka his sessionId where it is cookie based authentication. So, let's say it is a public forum, where everyone can login and give post, comment etc. I make a post and this input is not validated by the server for XSS check. The post contains a script (or even an image where this script is injected) where I make an AJAX request to send the session-id from the cookie of the other user's browser to my server. So, when everyone loads the post (or image of a cat), his sessionId will come to my browser. Now, I have the session-id, so I can make further requests on behalf of the user and server will accept this. Because this sessionId is my only identifier. So, how I inject a script tag to every other's computer is called XSS.
  - Resources - [Computerphile](https://www.youtube.com/watch?v=T1QEs3mdJoc&t=88s&ab_channel=Computerphile), [Computerphile2](https://www.youtube.com/watch?v=L5l9lSnNMxg&ab_channel=Computerphile)

- **Session vs Token authentication**