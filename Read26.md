# Android Fundamentals

## Introduction
#### Android is an operating system that is built basically for Mobile phones. It is based on the Linux Kernel and other open-source software and is developed by Google. It is used for touchscreen mobile devices such as smartphones and tablets. But nowadays these are used in Android Auto cars, TV, watches, camera, etc. It has been one of the best-selling OS for smartphones. Android OS was developed by Android Inc. which Google bought in 2005. Various applications (apps) like games, music player, camera, etc. are built for these smartphones for running on Android. Google Play store features more than 3.3 million apps. The app is developed on an application known as Android Studio. These executable apps are installed through a bundle or package called APK(Android Package Kit). 


## Android Application Components
### The basic components of an Android application are:

### 1. Activities
#### An activity is a class that is considered as an entry point for users that represents a single screen. A messenger application might have an activity that shows a new notification, another activity which reads messages and another which composes a new message. Each activity is independent of one another. For example – camera application can be started in an email application to compose an email that shares an image. The picture below depicts how each new activity adds an item to back stack and how the current activity is destroyed and previous activity is resumed. We will study the life cycle of activity in detail in our Android Activity article.

![Activities](https://user-images.githubusercontent.com/97638932/164999961-695b6a0a-3656-407f-a32d-6b4b29b24e48.png)

[Source](https://developer.android.com/guide/components/activities/activity-lifecycle)

### 2. Services
#### A service is a component that runs in the background, it acts as an invisible worker of our application. It keeps updating data sources and activities. It also broadcasts intents and performs tasks when applications are not active. An example of service is we can surf the internet or use any other application while listening to music.


### 3. Content Providers
#### Content Provider is a component that allows applications to share data among multiple applications. It hides the details of the database and can be used to read and write private data of the application which is not shared. It would be a mess to access data from other applications without content providers. For example – you can consider looking for contact details in contact list. Or You might want photos from the gallery which are also provided by Content Provider.


### 4. Broadcast Receiver
#### Broadcast Receiver is a component that responds to broadcast messages from another application or the same system. It can also deliver broadcasts to applications that are not running. For example – notify the user that the battery is low. Android developers can use broadcast messages in the application or outside the normal flow.
