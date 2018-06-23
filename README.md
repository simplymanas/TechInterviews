# Tech Interviews
### Frequently asked questions in Tech Interviews


## Difference between JWT (Java Web Tokens) & Oauth

### links

[jwt-vs-oauth](https://community.apigee.com/questions/21139/jwt-vs-oauth.html)

[RFC7519](https://tools.ietf.org/html/rfc7519)



| JWT | OAuth |
|--|--|
| its a token, JSON Web Token (JWT) is a compact, URL-safe means of representing claims to be transferred between two parties | its a framework to dispense token  |
| JWT is a different kind of OAuth token | OAuth token is not the only token
| is not a pointer to information |  a pointer to information
| JWT contains real information, it can be large | can be small as its just a pointer
|JWT are self-validating" what they mean is, any holder of the JWT can open it, validate it, and then make authorization decisions based on the claims presented in it. | Oauth are not
|JWT supports "Federation" - anyone can generate a token, and anyone can read and validate a token . | used when there is no federation
| used when asynchrony is required|
|  security. Both are bearer tokens. Both need to be protected as secrets.|same
|useful for self authenticating tokens|
|has lot more context about the user, session - including the signature.|less context
|better at performance as no server call requried|server clal required|
|forced to have lower expiry times to these tokens, as they are valid till the pre-defined rules re valid|
