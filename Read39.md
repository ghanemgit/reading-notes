# Location

## Inroduction

#### Using the Google Play services location APIs, your app can request the last known location of the user's device. In most cases, you are interested in the user's current location, which is usually equivalent to the last known location of the device.

#### Specifically, use the fused location provider to retrieve the device's last known location. The fused location provider is one of the location APIs in Google Play services. It manages the underlying location technology and provides a simple API so that you can specify requirements at a high level, like high accuracy or low power. It also optimizes the device's use of battery power.

#### Note: When your app is running in the background, access to location should be critical to the core functionality of the app and is accompanied with proper disclosure to users.

#### This lesson shows you how to make a single request for the location of a device using the getLastLocation() method in the fused location provider.

## Android - Location Based Services

#### This becomes possible with the help of Google Play services, which facilitates adding location awareness to your app with automated location tracking, geofencing, and activity recognition.

#### This tutorial shows you how to use Location Services in your APP to get the current location, get periodic location updates, look up addresses etc.

## The Location Object
#### The Location object represents a geographic location which can consist of a latitude, longitude, time stamp, and other information such as bearing, altitude and velocity. There are following important methods which you can use with Location object to get location specific information −

## Get the Current Location
#### To get the current location, create a location client which is LocationClient object, connect it to Location Services using connect() method, and then call its getLastLocation() method. This method returns the most recent location in the form of Location object that contains latitude and longitude coordinates and other information as explained above. To have location based functionality in your activity, you will have to implement two interfaces −

- GooglePlayServicesClient.ConnectionCallbacks
- GooglePlayServicesClient.OnConnectionFailedListener
#### These interfaces provide following important callback methods, which you need to implement in your activity class [here](https://www.tutorialspoint.com/android/android_location_based_services.htm)
