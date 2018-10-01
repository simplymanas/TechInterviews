# Tech Interviews
### Frequently asked questions in Tech Interviews

### Design

https://github.com/shashank88/system_design

http://highscalability.com/blog/2014/2/26/the-whatsapp-architecture-facebook-bought-for-19-billion.html

https://github.com/donnemartin/system-design-primer

https://medium.com/kokster/highly-available-redis-architecture-613c89f887b4

https://hackernoon.com/top-10-system-design-interview-questions-for-software-engineers-8561290f0444

http://highscalability.com/blog/2014/2/26/the-whatsapp-architecture-facebook-bought-for-19-billion.html

https://medium.com/@shivangsarawagi/design-an-online-movie-ticket-booking-system-like-bookmyshow-com-a247214a63e3

https://medium.com/netflix-techblog/system-architectures-for-personalization-and-recommendation-e081aa94b5d8?_sm_au_=iVVV1H5rMRH7P7NQ

https://medium.com/netflix-techblog/full-cycle-developers-at-netflix-a08c31f83249

https://github.com/sjuvekar/System-Design-Case-Studies/blob/master/studies/dropbox.md

### Scaling

http://www.erlang-factory.com/upload/presentations/558/efsf2012-whatsapp-scaling.pdf?_sm_au_=iVVV1H5rMRH7P7NQ

https://vimeo.com/44312354?_sm_au_=iVVV1H5rMRH7P7NQ


### Coding

https://www.geeksforgeeks.org/must-do-coding-questions-for-companies-like-amazon-microsoft-adobe/

https://github.com/donnemartin/interactive-coding-challenges

https://simpleprogrammer.com/programming-interview-questions/

https://hackernoon.com/50-data-structure-and-algorithms-interview-questions-for-programmers-b4b1ac61f5b0


### DDD

https://hackernoon.com/how-to-define-service-boundaries-251c4fc0f205

https://hackernoon.com/capability-mapping-and-context-mapping-95cf862f0753

### Coruses

https://www.safaribooksonline.com/videos/learn-design-patterns

https://www.safaribooksonline.com/videos/break-away-programming

https://www.safaribooksonline.com/videos/java-interview-guide

https://medium.com/the-coding-matrix/ddd-101-the-5-minute-tour-7a3037cf53b8

### JAVA

https://dzone.com/articles/top-10-java-interview-questions-that-i-recently-fa?edition=385432&utm_source=Weekly%20Digest&utm_medium=email&utm_campaign=Weekly%20Digest%202018-08-29

https://dzone.com/articles/java-copy-shallow-vs-deep-in-which-you-will-swim

### REST

https://restfulapi.net/

https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design


### Networking

https://career.guru99.com/top-100-networking-interview-questions-answers/


### Database

https://www.kdnuggets.com/2016/07/seven-steps-understanding-nosql-databases.html


### Process & Standard

https://engineering.videoblocks.com/these-four-clean-code-tips-will-dramatically-improve-your-engineering-teams-productivity-b5bd121dd150


### Almost Everything

https://github.com/andreis/interview

### Web Architecture 101

https://engineering.videoblocks.com/web-architecture-101-a3224e126947


## FAQ#1 : Difference between JWT (Java Web Tokens) & Oauth

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





## FAQ#2 : Difference between Container and VM

[differences](https://www.docker.com/what-container#/package_software)

|Container |VM
|--|--|
|Shares the OS and resources|A full virtualized system gets its own set of resources allocated to it, and does minimal sharing.|
|If you just want to isolate processes from each other and want to run a ton of them on a reasonably sized host, then Docker/LXC/runC seems to be the way to go.|If you want full isolation with guaranteed resources, a full VM is the way to go|
|![docker](https://www.docker.com/sites/default/files/Container%402x.png)|![VM](https://www.docker.com/sites/default/files/VM@2x.png)|
|**How containers works at low level?**   Each container runs in its own namespace but uses exactly the  _same_  kernel as all other containers. The isolation happens because kernel knows the namespace that was assigned to the process and during API calls it makes sure that process can only access resources in its own namespace. | **How virtualization works at low level?**    The net effect is that virtualization allows you to run two completely different OS on same hardware. Each guest OS goes through all the process of bootstrapping, loading kernel etc. You can have very tight security, for example, guest OS can't get full access to host OS or other guests and mess things up.|
|A virtual machine is a convenient way of packaging up virtual hardware, a kernel, and a user space. |A container, on the other hand, packages up only the user space; there is no kernel or virtual hardware.|
|![docker](https://rhelblog.files.wordpress.com/2015/09/user-space-vs-kernel-space-virtualization-vs-containerization11.png?w=640&h=254&zoom=2)|![VM](https://rhelblog.files.wordpress.com/2015/09/user-space-vs-kernel-space-virtualization-vs-containerization11.png?w=640&h=254&zoom=2)|
|Sharing an entire virtual machine with other developers can be inconvenient because of a virtual machine’s size and format|Containers have the advantage of providing developers, architects, quality engineering, release engineers, and systems administrators with a currency for collaboration that has the entire user space packaged and shipped in a convenient and easy to use format.|


## FAQ#3 : CAP Therorem

https://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed

## FAQ#4 : Difference between Redis and Memcache

https://stackoverflow.com/questions/10558465/memcached-vs-redis


