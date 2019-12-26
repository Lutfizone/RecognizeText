# RecognizeText
RecognizeText in Image with Firebase

# Create a New Firebase Project

1. Go to Firebase Console. All your previous Firebase projects will be listed here if you created one before.

2. Create a New Project.

3. After creating the project, Go to Project Settings. Choose "Android" as you platform. Then provide your app informations:

Android Package Name
App Name
Then click "Register App".

4. Download google-services.json file and place it into your Android app module root directory.

5. Time to add Firebase SDK into your app. There you'll see that Firebase wants you to add a classpath to your Project-level build.gradle file. I'm not giving it here cause the version changes and you should use the latest version.

6. Add apply plugin: 'com.google.gms.google-services' at the bottom of your app-level build.gradle file.

  dependencies {
    ...
	...
  }
  apply plugin: 'com.google.gms.google-services'
 

Alright, your app is now connected with your Firebase Project. If you didn't understand any step then follow the above video attached with this tutorial.

 

 

Recognize Text in Images (OCR) with ML Kit for Firebase
Now we'll move to our todays part. Firebase has different features like Google Analytics, Database, Storage, ML Kit, AdMob etc. Among them ML Kit is an integration of Google Cloud Vision. Close Vision is a huge development by Google such as you can perform object detection, face recognition, text recognition etc. In todays tutorial, we'll use the Text Recognition of Cloud Vision using Firebase ML Kit.

 

First of all, you will need to add the labrary for Firebase ML kit into your app-level build.gradle file.

dependencies {
    ...
	...
	implementation 'com.google.firebase:firebase-ml-vision:23.0.0'
}

# Demo
![recog](https://user-images.githubusercontent.com/29158899/71485511-f1086300-2843-11ea-8c83-5344b5a589cb.gif)
