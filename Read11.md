# Spring MVC
#### A Spring MVC is a Java framework which is used to build web applications. It follows the Model-View-Controller design pattern. It implements all the basic features of a core spring framework like Inversion of Control, Dependency Injection. A Spring MVC provides an elegant solution to use MVC in spring framework by the help of DispatcherServlet. Here, DispatcherServlet is a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.


## Spring Web Model-View-Controller

![Spring Web Model-View-Controller](https://user-images.githubusercontent.com/97638932/158474341-83481799-944b-4c37-8694-93ca0f459d71.png)


- Model - A model contains the data of the application. A data can be a single object or a collection of objects.
- Controller - A controller contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.
- View - A view represents the provided information in a particular format. Generally, JSP+JSTL is used to create a view page. Although spring also supports other view technologies such as Apache Velocity, Thymeleaf and FreeMarker.
- Front Controller - In Spring Web MVC, the DispatcherServlet class works as the front controller. It is responsible to manage the flow of the Spring MVC application.

## Advantages of Spring MVC Framework
### Let's see some of the advantages of Spring MVC Framework:-

- Separate roles - The Spring MVC separates each role, where the model object, controller, command object, view resolver, DispatcherServlet, validator, etc. can be fulfilled by a specialized object.
- Light-weight - It uses light-weight servlet container to develop and deploy your application.
- Powerful Configuration - It provides a robust configuration for both framework and application classes that includes easy referencing across contexts, such as from web controllers to business objects and validators.
- Rapid development - The Spring MVC facilitates fast and parallel development.
- Reusable business code - Instead of creating new objects, it allows us to use the existing business objects.
- Easy to test - In Spring, generally we create JavaBeans classes that enable you to inject test data using the setter methods.
- Flexible Mapping - It provides the specific annotations that easily redirect the page.

## Spring Web MVC Framework Example
#### You can see A get starting example [here](https://spring.io/guides/gs/serving-web-content/#scratch)
