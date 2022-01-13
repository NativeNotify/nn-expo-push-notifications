# nn-expo-push-notifications

```
### You must create a free NativeNotify.com account to receive an App Id and and App Token, or nn-expo-push-notifications won't work.
### Go to https://NativeNotify.com to sign up for free, no credit card required.
```

<br/>

## Install
```
npm i nn-expo-push-notifications 
<br/>
expo install expo-device expo-notifications
```

## Setup
Import registerNNPushToken in your App.js file:
```
import registerNNPushToken from 'nn-expo-push-notifications';
```
Paste this code into your App.js file:
```
let dataObject = registerNNPushToken(yourAppId, 'yourAppToken');
```
You must go to https://NativeNotify.com to receive a free App Id and App Token, or the registerNNPushToken function will not work. 
<br/><br/>
It's free to sign up. No credit card required.

<br/>

## Use
The registerNNPushToken will register your user's Native Notify push notification token and will return a data object. You can then send your users push notifications in the https://NativeNotify.com push notification portal.
<br/><br/>
You can send data objects with your Native Notify push notifications. Once a user taps on your Native Notify push notification, the value of the data object will be returned to this dataObject variable. You can use this value to do things like redirect your users to a particular screen once a Native Notify push notification is tapped.