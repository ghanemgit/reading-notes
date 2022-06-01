# Authentication with Amplify

## Getting started
#### The Amplify Auth category provides an interface for authenticating a user. Behind the scenes, it provides the necessary authorization to the other Amplify categories. It comes with default, built-in support for Amazon Cognito User Pool and Identity Pool. The Amplify CLI helps you to create and configure the auth category with an authentication provider.

## Goal
To setup and configure your application with Amplify Auth and go through a simple api to check the current auth session

## Prerequisites
#### An Android application targeting at least Android SDK API level 16 with Amplify libraries integrated For a full example of creating Android project, please follow the project setup walkthrough Configure Auth Category To start provisioning auth resources in the backend, go to your project directory and execute the command:

```amplify add auth```


#### Upon completion, amplifyconfiguration.json should be updated to reference provisioned backend auth resources. Note that these files should already be a part of your project if you followed the Project setup walkthrough.

## Install Amplify Libraries
#### Add the following dependency to your app's build.gradle along with others you added above in Prerequisites and click "Sync Now" when prompted:
```
dependencies {
    implementation 'com.amplifyframework:aws-auth-cognito:1.35.4'
}
```


## Initialize Amplify Auth
#### Add the Auth plugin before calling Amplify.configure. Update the code you added in Prerequisites:
````
// Add this line, to include the Auth plugin.
Amplify.addPlugin(new AWSCognitoAuthPlugin());
Amplify.configure(getApplicationContext());
````

## Check the current auth session
#### We can now check the current auth session. For testing purposes, you can run this from your MainActivity's onCreate method.

````
Amplify.Auth.fetchAuthSession(
    result -> Log.i("AmplifyQuickstart", result.toString()),
    error -> Log.e("AmplifyQuickstart", error.toString())
);
````

#### The isSignedIn property of the authSession will be false since we haven't signed in to the category yet.
