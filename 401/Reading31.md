# Espresso

- **Espresso: is a testing framework for Android to make it easy to write reliable user interface tests. And it's very important for developers, who believe that automated testing is an integral part of the development lifecycle.**

- **Espresso has basically three components:**

    1. ViewMatchers - allows to find view in the current view hierarchy

    2. ViewActions - allows to perform actions on the views

    3. ViewAssertions - allows to assert state of a view.

- **Packages**
    1. espresso-core - Contains core and basic View matchers, actions, and assertions. See Basics and Recipes.
    2. espresso-web - Contains resources for WebView support.
    3. espresso-idling-resource - Espresso's mechanism for synchronization with background jobs.
    4. espresso-contrib - External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
    5. espresso-intents - Extension to validate and stub intents for hermetic testing.
    6. espresso-remote - Location of Espresso's multi-process functionality.


## Create UI tests with Espresso Test Recorder

- It's a tool lets us create UI tests for the app without writing any test code, just by creating test scenario.
- Interact with the app and record that, then add assertations to verify UI elements in particular snapshots of the app.
- After that, Espresso Test Recorder takes the saved recording and automatically generates a corresponding UI test that we can run to test our app.

> Note: Turn off animations on the test device: Before using Espresso Test Recorder, make sure you turn off animations on your test device to prevent unexpected results.

- **Espresso tests consist of two primary components:**
1. UI interactions: It includes tap and type actions that a person may use to interact with the app.
2. Assertions on View elements: verify the existence or contents of visual elements on the screen.

- **To make the test**
1. Record UI interactions
2. Add assertions to verify UI elements
3. Save a recording
4. Run an Espresso test locally or Run an Espresso test with Firebase Test Lab for Android.

### Resources
- https://developer.android.com/training/testing/espresso
- https://developer.android.com/studio/test/espresso-test-recorder