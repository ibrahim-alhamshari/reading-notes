# Allowing Other Apps to Start an Activity

- **To perform an action from another app, my app should be prepared to respond to action requests by specifying the appropriate intent filter in my activity.**

- Ex: If I build a social app that can share messages or photos with the user's friends, I should support the `ACTION_SEND` intent. Then, when users initiate a "share" action from another app, the app appears as an option in the chooser dialog.
- To allow other apps to start my activity, I need to add an `<intent-filter>` element in the manifest file for the corresponding `<activity>` element.

- In order to define which intents my activity can handle properly, each intent filter I add should be as specific as possible in terms of the type of **action** and **data** the activity accepts.

> The system will send the given Intent to an activity if that activity has an intent filter that has the following intent's objects:
1. Action: Like --> `<action android:name="android.intent.action.SENDTO"/>` 
2. Data: like--> ` <category android:name="android.intent.category.DEFAULT"/>`
3. Category: Like--> `<data android:scheme="sms" />`

### Handle the Intent in my Activity
- As my activity starts, I need to call `getIntent()` to retrieve the Intent that started the activity. I can do so at any time during the lifecycle of the activity, but I should generally do so during early callbacks such as `onCreate()` or `onStart()`.

### Return a Result
- `setResult(RESULT_COLOR_RED);`
- `finish();`

### Resources
- [Intent Filters](https://developer.android.com/training/basics/intents/filters)