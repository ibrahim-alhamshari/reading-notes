# Android

- We use three languages to write it, which are *Kotlin, Java, and C++* languages. The Android SDK tools compile the code and the resource files into APK or Android App Bundle. An Android App Bundle, which is an archive file with an `.aab` suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime. 

**Each Android app lives in its own security sandbox, protected by the following Android security features:**
1. By default, every app runs in its own Linux process. 
2. Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.
3. The Android operating system is a multi-user Linux system in which each app is a different user.
4. By default, the system assigns each app a unique Linux user ID (the ID is used only by the system and is unknown to the app). The system sets permissions for all the files in an app so that only the user ID assigned to that app can access them.

> Least privilege: It's a principle the Android system uses, and it means that each app by default has access only to the components that it requires to do its work and no more. This creates a very secure environment in which an app cannot access parts of the system for which it is not given permission.

### App components
It's a very important building blocks for an android app. Each component is an entry point through which the user or the system can enter the app.

**There are four different types of app components:**
1. Activities: It is the entry point for interacting with the user. It represents a single screen with a user interface.
2. Services: It is a general-purpose entry point for keeping an app running in the background for all kinds of reasons. It is a component that runs in the background to perform long-running operations or to perform work for remote processes. A service does not provide a user interface.
3. Broadcast receivers: It is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
4. Content providers: It manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access.

### Activating components
- Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent.

- An intent: is an abstract description of an operation to be performed. It can be used with startActivity to launch an Activity, broadcastIntent to send it to any interested BroadcastReceiver components.


### The manifest file
- It declares the app's components. and does the following:
1. Identifies any user permissions the app requires
2. Declares the minimum API Level required by the app, based on which APIs the app uses.
3. Declares hardware and software features used or required by the app
4. Declares API libraries the app needs to be linked against (other than the Android framework APIs)

### Resources
- https://developer.android.com/guide/components/fundamentals