## Android 2
### Presenter: Joanna Chen

**Target Audience:** 
- Experienced hackers with some development experience

**Suggested Prerequisites:** 
- Development experience, be it mobile or web dev
 
**Workshop Goals:**
- Create a multi-activity Android app
 
**Description:**

Further finesse your Android skills with more advanced Android concepts and knowledge. In this workshop, you will learn about:
- The Android activity lifecycle
- How to pass data between activities
- Running a functioning multi-activity app

**Content Breakdown:**
- Setting up first activity from Android 1 or cloning from GitHub
- Explaining Android lifecycle & walking through lifecycle
- Creating another activity and passing data
- Using the data, either open camera or display some TextView
- Q&A

**Key Notes:**
* Android Lifecycle 
    * onCreate() - activity created, all the normal setup happens (views, data population), Bundle from activity’s previously frozen state is obtained, followed by onStart()
    * onRestart() - if activity stopped and started again
    * onStart() - activity is visible to user 
    * onResume() - activity is interacting with user, activity is at the top of the activity stack
    * onPause() - activity is in background, but not killed 
    * onStop() - activity no longer visible to user, next is either onRestart() or onDestroy()
    * onDestroy() - last call before activity is destroyed 

* Opening another activity
    * Create a new intent with the class of the activity that you want to go to 
    * Call startActivity(intent) to push the user to the new activity
    * To carry any data over to the new activity from the old one, put it in a Bundle and add it to the intent 
    * intent.putExtras(“key”, “value”);
    * In the new activity, call getIntent().getExtras() to get the Bundle with the information and parse the data you passed 

**[Slides](https://docs.google.com/presentation/d/1y4i5Xp9gnhDlRnCHXAHhfjvx3MKwnh3D48TEhDL8soY/edit?usp=sharing)**
 

