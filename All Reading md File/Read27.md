# Intents, Activities, and SharedPreferences

## Introduction
#### When doing a job, users engage with a task, which is a set of actions. The activities are stacked in the order in which they are opened in a stack called the back stack. One action in an email app, for example, maybe to display a list of fresh messages. When the user picks a message, a new activity appears in which the user may read the message. This new action has been sent to the back of the queue. When the user clicks the Back button, the new action is completed and removed from the stack. When numerous applications are running in a multi-windowed environment, which is allowed in Android 7.0 (API level 24) and above, the system maintains tasks for each window individually; each window may contain several tasks. The system organizes tasks, or groups of tasks, on a per-window basis for Android apps running on Chromebooks.

![article-660x339](https://user-images.githubusercontent.com/97638932/165188373-a36692ac-afff-4398-9120-bcc5a5c9cc8b.png)

## Task Stacks Everywhere
#### A "task" is a collection of activities stemming from a "root" application. This group is cohesive and when the user hits the home screen, the entire "task" is moved to the background until the stack is re-activated. While in the background, all the activities in the task are stopped, but the back stack for the task remains intact. If the user were to open another separate application now, that app would have an entirely separate task stack that would come to the foreground. This means that multiple discrete stacks frequently are stored by the system. There might be several task stacks in the background and when the user re-enters the related application, that stack will reappear in the foreground with states restored.

## Multiple Activity Instances
#### This process of multiple task stacks is just the beginning. The real point of understanding comes from exploring what happens when we launch the same activity multiple times. Because the activities in the back stack are never rearranged, every time an activity is started via an intent, a brand new instance of that activity is created and pushed onto the stack. This means that if you have an activity (say the timeline for twitter), and you launch the timeline activity multiple times using different intents, then multiple instances of that activity will be tracked in the stack.

#### This gets even more complex when you consider you might launch the same Activity from multiple different task stacks. For example, think about how many apps might launch the browser and how many instances of a browser you might have across all task stacks. By default, if the user navigates backward using the Back button, each instance of the activity is revealed in the order in which they were opened (each with their own UI state). See Tasks and Back Stack official guide for the source of the above content and additional details.





## Android SharedPreferences
#### Android provides many ways of storing data of an application. One of this way is called Shared Preferences. Shared Preferences allow you to save and retrieve data in the form of key,value pair. In order to use shared preferences, you have to call a method getSharedPreferences() that returns a SharedPreference instance pointing to the file that contains the values of preferences.

You can save something in the sharedpreferences by using SharedPreferences.Editor class. You will call the edit method of SharedPreference instance and will receive it in an editor object. Its syntax is −
```
Editor editor = sharedpreferences.edit();
editor.putString("key", "value");
editor.commit();
ADVERTISEMENT BY ADRECOVER
```
Apart from the putString method , there are methods available in the editor class that allows manipulation of data inside shared preferences. 





