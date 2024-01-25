Dessert Clicker app
=====================

Code for Android Basics with Compose Codelab.

Introduction
------------

Dessert Clicker is a game about making desserts.

Press the button, make a dessert, earn the big bucks.

You use this app in the course to explore the Android lifecycle and log messages to
the Android console (Logcat).

Pre-requisites
--------------

You need to know:
- How to open, build, and run apps with Android Studio.
- What an activity is, and how to create one in your app.
- What the activity's onCreate() method does, and the kind of operations
  that are performed in that method.


Getting Started
---------------

1. Download and run the app.

### Personal Notes

1. The asterisk on the onRestart() method indicates that this method is not called every time the state transitions between Created and Started. It is only called if onStop() was called and the activity is subsequently restarted.
2.  When you override the onCreate() method, you must call the superclass implementation to complete the creation of the Activity, so within it, you must immediately call super.onCreate(). The same is true for other lifecycle callback methods.
3. Because you used MainActivity as the log tag in your code, you can use that tag to filter the log. Your log message includes the date and time, your log tag, the name of the package
4. onCreate() when the system creates the app.
   onStart() makes the app visible on the screen, but the user is not yet able to interact with it.
   onResume() brings the app to the foreground, and the user is now able to interact with it.
5. The part of the lifecycle in which the app is fully onscreen and has user focus is called the foreground lifetime.
6. Whatever code runs in onPause() blocks other things from displaying, so keep the code in onPause() lightweight. For example, if a phone call comes in, the code in onPause() may delay the incoming-call notification.
7. we Should declare a tag at start of each activity to use in logging to represent the activity name.
8. he priority of the log message, that is, how important the message is. In this case, the Log.v() logs verbose messages. Log.d() method writes a debug message. Other methods in the Log class include Log.i() for informational messages, Log.w() for warnings, and Log.e() for error messages.
9. Make sure user doesn't encounter any data loss when android os shutsdown the app due to lagging or danger due to lack of resources.. using states.
