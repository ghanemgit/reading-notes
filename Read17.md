# Spring Authorization

## Introduction
#### This guide is a primer for Spring Security, offering insight into the design and basic building blocks of the framework. We cover only the very basics of application security. However, in doing so, we can clear up some of the confusion experienced by developers who use Spring Security. To do this, we take a look at the way security is applied in web applications by using filters and, more generally, by using method annotations. Use this guide when you need a high-level understanding of how a secure application works, how it can be customized, or if you need to learn how to think about application security. This guide is not intended as a manual or recipe for solving more than the most basic problems (there are other sources for those), but it could be useful for beginners and experts alike. Spring Boot is also often referenced, because it provides some default behavior for a secure application, and it can be useful to understand how that fits in with the overall architecture.


![image](https://user-images.githubusercontent.com/97638932/161058457-98ab5168-003e-4c0d-b375-3fff34b882f4.png)


## Authentication and Access Control
#### Application security boils down to two more or less independent problems: authentication (who are you?) and authorization (what are you allowed to do?). Sometimes people say “access control” instead of "authorization", which can get confusing, but it can be helpful to think of it that way because “authorization” is overloaded in other places. Spring Security has an architecture that is designed to separate authentication from authorization and has strategies and extension points for both.


![image](https://user-images.githubusercontent.com/97638932/161058669-daec9f26-caec-4d18-9e43-810f30c3ce50.png)
