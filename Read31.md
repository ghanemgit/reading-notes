# Espresso


### Is UI Testing necessary?
#### Yes, it is very important to test the UI in all aspects so that the user will not get any trouble in using the application. The application should be easy to use. If the UI is tested properly it makes the usability of the application easier.

#### Test execution is much faster as compared to manual testing. It will reduce small design and development bugs and QA person’s headaches.


#### Espresso is a testing framework for Android to make it easy to write reliable user interface tests. Google released the Espresso framework in Oct. 2013. Since its 2.0 release Espresso is part of the Android Support Repository.

#### Espresso automatically synchronizes your test actions with the user interface of your application. The framework also ensures that your activity is started before the tests run. It also let the test wait until all observed background activities have finished. It is intended to test a single application but can also be used to test across applications. If used for testing outside your application, you can only perform black box testing, as you cannot access the classes outside of your application.

### Espresso has basically three components:

- ViewMatchers - allows to find view in the current view hierarchy.
- ViewActions - allows to perform actions on the views.
- ViewAssertions - allows to assert state of a view.

### Workflow of Espresso Testing Framework
![image](https://user-images.githubusercontent.com/97638932/167954411-35978583-4991-4384-bb25-27b1e26a08c0.png)

[source](https://medium.com/mindful-engineering/ui-testing-with-espresso-in-android-10dfbc9f25da)


### The advantages of UI tests are as follows

#### 1-Test scripts once created can be reused; this makes testing easily scalable.
#### 2-Improves performance as efficient test scripts deliver fast and accurate results.
#### 3-Simplified testing by letting QAs refer to previous builds/test results and proceed further.
#### 4-Machines are less prone to errors than humans, which leads to a higher likelihood of accurate results even with a large number of tests.



