## Tasks and the Back Stack
- **A task is a stack of activities that the user is concerned with. The activity at the bottom of the stack is called the base activity, and whatever activity is on top is the activity that the user sees. When you press the Back button, you are popping the top activity off of this stack.**

- When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. 
- When the user presses the Back button, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes (the previous state of its UI is restored).
- Activities in the stack are never rearranged, only pushed and popped from the stack—pushed onto the stack when started by the current activity and popped off when the user leaves it using the Back button.


![Tasks and Back Stack](https://docs.huihoo.com/android/3.0/images/fundamentals/diagram_backstack.png)

## Save key-value data
- To save the key's value, you have to use `SharedPreferences`.
- `SharedPreferences`: It is object points to a file containing key-value pairs and provides simple methods to read and write them.

### Resources
- https://developer.android.com/guide/components/activities/tasks-and-back-stack
- https://developer.android.com/training/data-storage/shared-preferences