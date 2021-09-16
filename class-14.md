# Authentication

> **Look to Table For easy understanding of the content and access to the desired (in order) :**

|name of subject      | Location On This Page|
|---------------------|---------------------|
|OAuth|First Paragraph|
|Authentication and Authorization Flows|Second Paragraph|
|lovers of reading|Third Paragraph|
|Things I want to know more about|In The Last|

---
## OAuth

* ### ***What Is OAuth ?*** 

OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization .


* ### ***OAuth history*** 

Created and strongly supported from the start by Twitter, Google and other companies, OAuth was released as an open standard in 2010 as RFC 5849, and quickly became widely adopted. Over the next two years, it underwent substantial revision, and version 2.0 of OAuth, was released in 2012 as RFC 6749. Even though version 2.0 was widely criticized for multiple reasons covered below, it gained even more popularity. Today, you can add Amazon, Facebook, Instagram, LinkedIn, Microsoft, Netflix, Paypal and a list of other internet who’s-whos as adopters .


![OAuth](https://res.cloudinary.com/practicaldev/image/fetch/s--X8na4LD9--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/qnoefye56zqd0vb5kar0.jpg)

* ### ***How OAuth works ?*** 

Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified) :

1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity .

2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved .

3. The first site gives this token and secret to the initiating user’s client software .

4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site) .

5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website .

6. The user approves (or their software silently approves) a particular transaction type at the first website .

7. The user is given an approved access token (notice it’s no longer a request token) .

8. The user gives the approved access token to the first website .

9. The first website gives the access token to the second website as proof of authentication on behalf of the user .

10. The second website lets the first website access their site on behalf of the user .

11. The user sees a successfully completed transaction occurring .

12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons) .

---
## Authentication and Authorization Flows

* ### ***Authorization Code Flow*** 

Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token .

![Authorization Flows](https://www.hackercitizen.com/content/images/2021/01/authentication-vs-authorization-min-1.png)

* ### ***Implicit Flow with Form Post*** 

As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication .

* ### ***Hybrid Flow*** 

Applications that are able to securely store Client Secrets may benefit from the use of the Hybrid Flow, which combines features of the Authorization Code Flow and Implicit Flow with Form Post to allow your application to have immediate access to an ID token while still providing for secure and safe retrieval of access and refresh tokens. This can be useful in situations where your application needs to immediately access information about the user, but must perform some processing before gaining access to protected resources for an extended period of time .

* ### ***Device Authorization Flow*** 

With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications .

---
## ***For lovers of reading*** :

<img src='https://www.lovereading.co.uk/content/images/love-reading-generic-facebook-image.jpg' height='300'>


**[More about Auth for single page apps ......](https://auth0.com/docs/libraries/auth0-react)**

**[More about OAuth ......](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)**

**[More about Authorization and Authentication flows ......](https://auth0.com/docs/authorization/flows)**

---
## Things I want to know more about

* ### ***Project Of Developer .***

---
#### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)

---
<b>
<p align="center">
© Mohammad alwrekat
</p>
