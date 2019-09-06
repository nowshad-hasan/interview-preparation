## Contents

* [Basic Things](#basic-things)
* [Advanced Android](#advanced-android)
* [Activity](#activity)
* [Fragments](#fragments)
* [Views and ViewGroups](#views-and-viewgroups)
* [Displaying Lists of Content](#displaying-lists-of-content)

### Basic things
#### Base
* Tell us `Android Application Components`.
    1. Activities
    2. Services
    3. Broadcast Receiver
    4. Content Provider

  Reference - [Developer Android](https://developer.android.com/guide/components/fundamentals.html#Components)

* What is the `Structure of an Android Application`?</br>
  Reference - [Developer Android](https://developer.android.com/studio/projects)
* What is `Context`? How is it used? </br>
  Reference - [MindOrks](https://blog.mindorks.com/understanding-context-in-android-application-330913e32514), [Gaurav in FreeCodeCamp](https://www.freecodecamp.org/news/mastering-android-context-7055c8478a22/).
* What is `AndroidManifest`? </br>
  Reference - [Developer Android](https://developer.android.com/guide/topics/manifest/manifest-intro)
* Describe `Activity Lifecycle`</br>
  Reference - [Developer Android](https://developer.android.com/guide/components/activities/activity-lifecycle)</br>
  Video - [Coding in Flow](https://www.youtube.com/watch?v=UJN3AL4tiqw), [Udacity](https://www.youtube.com/watch?v=85MppyLJHz0)

* What is `Application` class? [Codepath](https://github.com/codepath/android_guides/wiki/Understanding-the-Android-Application-Class), [Medium](https://medium.com/@balakrishnanpt/android-application-class-a8a1d64c82d1), [Developer Android](https://developer.android.com/reference/android/app/Application)

### Activity

* What is `Activity`? [MindOrks](https://blog.mindorks.com/android-activity-lifecycle)

* Explain `Activity` and `Fragment` lifecycle. (Complete diagram [GitHub](https://github.com/xxv/android-lifecycle), simplified diagram for [Activity](https://developer.android.com/guide/components/activities/activity-lifecycle.html#alc), [Fragment](https://developer.android.com/guide/components/fragments.html#Lifecycle)), [Activity lifecycle](https://blog.mindorks.com/android-activity-lifecycle) and [Fragments lifecycle](https://blog.mindorks.com/android-fragments-and-its-lifecycle)

* What are "launch modes"? [MindOrks](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)

### Fragments

* What is `Fragment`? [MindOrks](https://blog.mindorks.com/android-fragments-and-its-lifecycle)

* What is the difference between a `Fragment` and an `Activity`? Explain the relationship between the two.

* Why is it recommended to use only the default constructor to create a `Fragment`? [StackOverflow](https://stackoverflow.com/a/16042750/2809326)

* How would you communicate between two Fragments? [Android Official](https://developer.android.com/training/basics/fragments/communicating.html)

* What is retained `Fragment`? [AndroidDesignPatterns](https://www.androiddesignpatterns.com/2013/04/retaining-objects-across-config-changes.html)

### Views and ViewGroups

* What is `View` in Android? [MindOrks](https://blog.mindorks.com/android-user-interface-view-components)

* Difference between `View.GONE` and `View.INVISIBLE`? [StackOverflow](https://stackoverflow.com/questions/11556607/android-difference-between-invisible-and-gone)

* Can you create custom views? How? [MindOrks](https://blog.mindorks.com/create-your-own-custom-view)

* What are ViewGroups and how they are different from the Views?

* What is a canvas?

* What is a `SurfaceView`?

* Relative Layout vs Linear Layout. [MindOrks](https://blog.mindorks.com/android-layout-relative-linear-frame)

* Tell about Constraint Layout [MindOrks](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)

* Do you know what is the view tree? How can you optimize its depth?

#### Displaying Lists of Content

* What is the difference between `ListView` and `RecyclerView`? [Stackoverflow 1](https://stackoverflow.com/questions/28525112/android-recyclerview-vs-listview-with-viewholder/31199564), [Medium](https://medium.com/@manuaravindpta/what-is-the-difference-between-listview-and-recyclerview-bcd82c64ffbb), [Blog](https://www.thedroidsonroids.com/blog/what-is-the-difference-between-listview-recyclerview), [Stackoverflow 2](https://stackoverflow.com/questions/26728651/recyclerview-vs-listview), [Udacity](https://www.youtube.com/watch?v=-VPM6ICgCk8), [Stackoverflow 3](https://stackoverflow.com/questions/11945563/how-listviews-recycling-mechanism-works)

* What is the ViewHolder pattern? Why should we use it?[Javacodegeeks](https://www.javacodegeeks.com/2013/09/android-viewholder-pattern-example.html), [Stackoverflow](https://stackoverflow.com/questions/21501316/what-is-the-benefit-of-viewholder-pattern-in-android)

* What is `SnapHelper`? [MindOrks](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)

#### Dialogs and Toasts

* What is `Dialog` in Android? [Developer android](https://developer.android.com/guide/topics/ui/dialogs)

* What is `Dialog Fragment` in Android?[Codepath](https://guides.codepath.com/android/using-dialogfragment), [Developer android](https://developer.android.com/reference/android/support/v4/app/DialogFragment.html), [Journaldev](https://www.journaldev.com/23096/android-dialogfragment), [MindOrks](https://blog.mindorks.com/implementing-dialog-fragment-in-android)

* What is `Toast` in Android? [Developer android](https://developer.android.com/guide/topics/ui/notifiers/toasts#java), [Stackoverflow](https://stackoverflow.com/questions/3308975/button-in-custom-android-toast)

* What the difference between `Dialog` and `Dialog Fragment`? [Stackoverflow](https://stackoverflow.com/questions/13765127/dialogfragment-advantages-over-alertdialog/13765411)


#### Intents and Broadcasting

* What is `Intent`? [StackOverflow](https://stackoverflow.com/questions/6578051/what-is-an-intent-in-android), [Developer android](https://developer.android.com/guide/components/intents-filters), [Vogella](https://www.vogella.com/tutorials/AndroidIntent/article.html)

* What is an Implicit `Intent`?	[StackOverflow](https://stackoverflow.com/questions/10272699/what-is-the-different-between-explicit-and-implicit-activity-call-in-android/20728603)


* What is a `BroadcastReceiver`? [StackOverflow](https://stackoverflow.com/questions/5296987/what-is-broadcastreceiver-and-when-we-use-it), [Developer android](https://developer.android.com/guide/components/broadcasts), [Vogella](https://www.vogella.com/tutorials/AndroidBroadcastReceiver/article.html), [Broadcast  Exceptions](https://developer.android.com/guide/components/broadcast-exceptions)

* What is a `LocalBroadcastManager`? [Developer Android](https://developer.android.com/reference/android/support/v4/content/LocalBroadcastManager.html)

* What is the function of an `IntentFilter`? [StackOverflow](https://stackoverflow.com/questions/3321514/what-are-intent-filters-in-android)

* What is a Sticky `Intent`? [AndroidInterview](http://www.androidinterview.com/what-is-a-sticky-intent/)

* Describe how broadcasts and intents work to be able to pass messages around your app? [Techotopia](https://www.techotopia.com/index.php/Android_Broadcast_Intents_and_Broadcast_Receivers)

* What is a `PendingIntent`? [Stackoverflow](https://stackoverflow.com/questions/2808796/what-is-an-android-pendingintent), [Developer android](https://developer.android.com/reference/android/app/PendingIntent), [Video - Developer android](https://www.youtube.com/watch?v=-iog_fmm6mE), [Blog](https://android.jlelse.eu/intent-vs-pendingintent-8ef2ad5824ed), [Medium](https://medium.com/@architgupta690/creating-pending-intent-in-android-a-step-by-step-guide-74784ec60c9e), [Journaldev](https://www.journaldev.com/10463/android-notification-pendingintent)

* What are the different types of Broadcasts? [Blog](https://www.edureka.co/blog/android-tutorials-broadcast-receivers/)

### Services

* What is `Serivce`? [Developer Android](https://developer.android.com/guide/components/services), [Javatpoint](https://www.javatpoint.com/android-service-tutorial), [Tutorialspoint](https://www.tutorialspoint.com/android/android_services.htm), [Vogella](https://www.vogella.com/tutorials/AndroidServices/article.html), [Proandroiddev](https://proandroiddev.com/deep-dive-into-android-services-4830b8c9a09), [Tutlane](https://www.tutlane.com/tutorial/android/android-services-with-examples), [MindOrks](https://medium.com/mindorks/mastering-android-service-of-2018-a4a1df5ed5a6), [Blog 1](https://androidclarified.com/android-service-lifecycle-and-working/), [Blog 2](https://www.survivingwithandroid.com/android-service-tutorial-2/)

* `Service` vs `IntentService`. [StackOverflow](https://stackoverflow.com/a/15772151/5153275), [MindOrks](https://blog.mindorks.com/service-vs-intentservice-in-android)

* What is a `JobScheduler`? [Vogella](http://www.vogella.com/tutorials/AndroidTaskScheduling/article.html), [Developer android](https://developer.android.com/reference/android/app/job/JobScheduler), [Medium](https://medium.com/google-developers/scheduling-jobs-like-a-pro-with-jobscheduler-286ef8510129)

#### Inter-process Communication

* How can two distinct Android apps interact?  [Developer Android](https://developer.android.com/training/basics/intents)

* Is it possible to run an Android app in multiple processes? How?

* What is AIDL? Enumerate the steps in creating a bounded service through AIDL. [Developer Android](https://developer.android.com/guide/components/aidl)

* What can you use for background processing in Android?  [Developer Android](https://developer.android.com/guide/background)

* What is a `ContentProvider` and what is it typically used for? [Developer Android](https://developer.android.com/guide/topics/providers/content-provider-basics) [Developer Android](https://developer.android.com/guide/topics/providers/content-providers)

#### Long-running Operations

* How would you perform a long-running operation in an application?

* Why should you avoid to run non-ui code on the main thread?

* What is ANR? How can the ANR be prevented? [Developer Android](https://developer.android.com/topic/performance/vitals/anr.html)

  - ANR timing - 5 seconds


* What is an `AsyncTask`?  [Developer Android](https://developer.android.com/reference/android/os/AsyncTask)

* What are the problems in asynctask? [Blog 1](https://blog.danlew.net/2014/06/21/the-hidden-pitfalls-of-asynctask/), [Blog 2](https://medium.com/@akhilgupta.me/asynctask-memory-leaks-170f4a21b16f)

* When would you use java thread instead of an asynctask?[Developer android](https://developer.android.com/topic/performance/threads), [Medium](https://medium.com/@varun93342/difference-between-thread-service-and-asynctask-in-android-d6e37960e56c)

* What is a `Loader`? (Depricated) [Developer Android](https://developer.android.com/guide/components/loaders)

* What is the relationship between the life cycle of an `AsyncTask` and an `Activity`? What problems can this result in? How can these problems be avoided?

* Explain `Looper`, `Handler` and `HandlerThread`. [MindOrks](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a) and [MindOrks Video](https://www.youtube.com/watch?v=rfLMwbOKLRk&list=PL6nth5sRD25hVezlyqlBO9dafKMc5fAU2), [Dev.to](https://dev.to/anuj/understanding-handler-looper-and-handler-thread-3anf), [Medium](https://medium.com/quark-works/how-to-use-thread-looper-and-handler-in-android-c0532f15b03e)

### Working With Multimedia Content

* How do you handle bitmaps in Android as it takes too much memory? [Developer Android](https://developer.android.com/topic/performance/graphics/load-bitmap) [Developer Android](https://developer.android.com/topic/performance/graphics/manage-memory)

* What is the difference between a regular `Bitmap` and a nine-patch image?

* Tell about the `Bitmap` pool. [MindOrks](https://blog.mindorks.com/how-to-use-bitmap-pool-in-android-56c71a55533c)

* How to play sounds in Android? [Vogella](http://www.vogella.com/tutorials/AndroidMedia/article.html)

### Data Saving

* How to persist data in an Android app? [MindOrks](https://blog.mindorks.com/android-shared-preferences-in-kotlin)

* What is ORM? How does it work? [DZone](https://dzone.com/articles/a-quick-guide-to-using-popular-orm-for-android-dev)

  ORM means Object relational mapping. We store data in database row-wise. But in our project level we always work with object. So, ORM DB gives us an opportunity to map the object with table row. It makes query easier.

* How would you preserve `Activity` state during a screen rotation? [StackOverflow](https://stackoverflow.com/questions/3915952/how-to-save-state-during-orientation-change-in-android-if-the-state-is-made-of-m), [Android jlelse](https://android.jlelse.eu/handling-orientation-changes-in-android-7072958c442a), [Developer Android](https://developer.android.com/guide/topics/resources/runtime-changes), [Medium by Joanna Smith](https://medium.com/google-developers/activity-revival-and-the-case-of-the-rotating-device-167e34f9a30d), [Medium](https://medium.com/hootsuite-engineering/handling-orientation-changes-on-android-41a6b62cb43f), [Medium by Lyla Fujiwara](https://medium.com/androiddevelopers/viewmodels-persistence-onsaveinstancestate-restoring-ui-state-and-loaders-fc7cc4a6c090)

* What are different ways to store data in your Android app? [Developer Android](https://developer.android.com/guide/topics/data/data-storage)

### Memory Optimizations

* What is the `onTrimMemory()` method? [Developer Android](https://developer.android.com/topic/performance/memory)

    Called when the operating system has determined that it is a good time for a process to trim unneeded memory from its process. This will happen for example when it goes in the background and there is not enough memory to keep as many background processes running as desired

* How does the OutOfMemory happens? [Geeksforgeeks](https://www.geeksforgeeks.org/understanding-outofmemoryerror-exception-java/)

  Thrown when the Java Virtual Machine cannot allocate an object because it is out of memory, and no more memory could be made available by the garbage collector

* How do you find memory leaks in Android applications? [MindOrks](https://mindorks.com/blog/detecting-and-fixing-memory-leaks-in-android)

### Battery Life Optimizations

* How to reduce battery usage in an android application? [MindOrks](https://blog.mindorks.com/battery-optimization-for-android-apps-f4ef6170ff70)

* What is Doze? What about App Standby? [Developer Android](https://developer.android.com/training/monitoring-device-state/doze-standby)

* What is `overdraw`? [Developer Android](https://developer.android.com/topic/performance/rendering/overdraw.html)

### Supporting Different Screen Sizes

* How did you support different types of resolutions? [Developer android - screens support](https://developer.android.com/guide/practices/screens_support), [Developer android - compatibility](https://developer.android.com/guide/practices/compatibility), [Developer android - screensizes](https://developer.android.com/training/multiscreen/screensizes)

### Permissions

* What are the different protection levels in permission? [Developer android](https://developer.android.com/guide/topics/permissions/overview)

### Native Programming

* What is the NDK and why is it useful? [MindOrks](https://www.youtube.com/watch?v=iljxHVt7Arc)

* What is renderscript? [MindOrks](https://blog.mindorks.com/comparing-android-ndk-and-renderscript-1a718c01f6fe)

### Android System Internal

* What is the Dalvik Virtual Machine? [Javatpoint](https://www.javatpoint.com/dalvik-virtual-machine)

* What is the difference between JVM, DVM and ART? [AndroidPub](https://android.jlelse.eu/closer-look-at-android-runtime-dvm-vs-art-1dc5240c3924), [Journaldev](https://www.journaldev.com/23464/android-runtime-dvm-vs-art-aot-vs-jit), [Stackoverflow](https://stackoverflow.com/questions/31957568/what-is-difference-between-dvm-and-art-why-dvm-has-been-officially-replaced-wi)

* What are the differences between Dalvik and ART? [MindOrks](https://blog.mindorks.com/what-are-the-differences-between-dalvik-and-art), [Blog](https://infinum.co/the-capsized-eight/art-vs-dalvik-introducing-the-new-android-runtime-in-kit-kat), [Quora](https://www.quora.com/What-is-the-difference-between-ART-and-Dalvik-in-Android)

* What is DEX? [Stackoverflow](https://stackoverflow.com/questions/7750448/what-are-dex-files-in-android), [Developer android - DexFile](https://developer.android.com/reference/dalvik/system/DexFile), [Developer android - Multidex](https://developer.android.com/studio/build/multidex)

* Can you manually call the Garbage collector? [Stackoverflow](https://stackoverflow.com/questions/3117429/garbage-collector-in-android), [Blog](https://www.coderzheaven.com/2017/09/05/do-we-need-to-call-the-garbage-collector-manually-in-android/), [Developer android](https://developer.android.com/topic/performance/memory-overview), [DZone](https://dzone.com/articles/understanding-android-gc-logs)

### Debugging and Programming Tools

* What is ADB? [Developer android](https://developer.android.com/studio/command-line/adb)

* What is DDMS and what can you do with it? [Toptal](https://www.toptal.com/android/android-ddms-ultimate-power-console), [Developer android](https://developer.android.com/studio/profile/monitor)

* What is the StrictMode? [MindOrks](https://blog.mindorks.com/use-strictmode-to-find-things-you-did-by-accident-in-android-development-4cf0e7c8d997)

* What is Lint? What is it used for?

### Others

* Why Bundle class is used for data passing and why cannot we use simple Map data structure [Developer android](https://developer.android.com/guide/components/activities/parcelables-and-bundles)

* How do you troubleshoot a crashing application?

* Explain Android notification system. [Developer android](https://developer.android.com/guide/topics/ui/notifiers/notifications), [Material design](https://material.io/design/platform-guidance/android-notifications.html)

* What is the difference between Serializable and Parcelable? Which is the best approach in Android?

* Have you developed widgets? Describe. [MindOrks](https://blog.mindorks.com/android-widgets-ad3d166458d3)

* What is AAPT? [Developer android](https://developer.android.com/studio/command-line/aapt2), [Stackoverflow](https://stackoverflow.com/questions/28234671/what-is-aapt-android-asset-packaging-tool-and-how-does-it-work/49259810)

* What is the best way to update the screen periodically? [Codepath](https://guides.codepath.com/android/Repeating-Periodic-Tasks), [AndroidPub](https://android.jlelse.eu/refreshing-views-periodically-in-android-57a429949ceb)

* FlatBuffers vs JSON. [MindOrks](https://blog.mindorks.com/why-consider-flatbuffer-over-json-2e4aa8d4ed07)

* `HashMap`, `ArrayMap` and `SparseArray` [MindOrks](https://blog.mindorks.com/android-app-optimization-using-arraymap-and-sparsearray-f2b4e2e3dc47)

* What are Annotations? [MindOrks](https://blog.mindorks.com/creating-custom-annotations-in-android-a855c5b43ed9), [Link](https://blog.mindorks.com/improve-your-android-coding-through-annotations-26b3273c137a), [Video](https://www.youtube.com/watch?v=LEb9if2HHSw)

* How to handle multi-touch in android [GitHub](https://arjun-sna.github.io/android/2016/07/20/multi-touch-android/)

* How to implement XML namespaces? [Developer android](https://developer.android.com/reference/javax/xml/namespace/NamespaceContext)

* What is the support library? Why was it introduced?[MartianCraft](http://martiancraft.com/blog/2015/06/android-support-library/)

* What is Android Data Binding? [Developer Android](https://developer.android.com/topic/libraries/data-binding/index.html)

* What are Android Architecture Components? [MindOrks](https://blog.mindorks.com/what-are-android-architecture-components)

* How to implement search using RxJava operators? [MindOrks](https://blog.mindorks.com/implement-search-using-rxjava-operators-c8882b64fe1d)

### Architecture

* Describe the architecture of your last app.

* Describe MVP. [MindOrks](https://mindorks.com/course/android-mvp-introduction)

* What is presenter?

* What is model?

* Describe MVC.

* Describe MVI

* Describe the repository pattern

* What is controller?

* Describe MVVM. [GitHub](https://github.com/MindorksOpenSource/android-mvvm-architecture)

* Tell something about clean code [MindOrks](https://blog.mindorks.com/every-programmer-should-read-this-book-6755dedec78d)


### Design Problem

* Design Uber App.

* Design Facebook App.

* Design Facebook Near-By Friends App.

* Design WhatsApp.

* Design SnapChat.

* Design problems based on location based app.


### Tools And Technologies

* Git. [MindOrks Youtube](https://www.youtube.com/watch?v=D4h8Dbrjt4M&list=PL6nth5sRD25itbyNVUULAebzL-VLrLfkK)

* RxJava. [MindOrks](https://blog.mindorks.com/a-complete-guide-to-learn-rxjava-b55c0cea3631)

* Dagger 2. [MindOrks](https://blog.mindorks.com/a-complete-guide-to-learn-dagger-2-b4c7a570d99c)

* Android Development Useful Tools. [MindOrks](https://blog.mindorks.com/android-development-useful-tools-fd73283e82e3)

* Firebase. [Firebase.google.com](https://firebase.google.com/)


### Android Test Driven Development

* What is Espresso? [Developer Android](https://developer.android.com/training/testing/ui-testing/espresso-testing.html)

* What is Robolectric? [Robolectric](http://robolectric.org/)

* What are the disadvantages of using Roboelectric?

* What is UI-Automator? [Developer Android](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html)

* Explain unit test.

* Explain instrumented test.

* Have you done unit testing or automatic testing?

* Why Mockito is used? [Official site](http://site.mockito.org/)

* Describe JUnit test.


### Others

* What is Android Jetpack? [MindOrks](https://blog.mindorks.com/what-is-android-jetpack-and-why-should-we-use-it)

* Describe how REST APIs work. What is REST?

* Describe other forms of web API architecutre. [GraphQL] (https://medium.com/mindorks/what-is-graphql-and-using-it-on-android-ab8e493abdd7) [SOAP] (https://www.w3.org/TR/ws-arch/)

* Describe SQLite. [MindOrks](https://blog.mindorks.com/android-sqlite-database-in-kotlin)

* Describe database.

* Project Management tool - trello, basecamp, kanban, jira, asana.

* About build System - gradle, maven, ant, buck.

* About multiple apk for android application. [MindOrks](https://mindorks.com/blog/how-to-create-multiple-apk-files-for-android-application)

* Reverse Engineering an APK.

* What is proguard used for? [MindOrks](https://blog.mindorks.com/applying-proguard-in-an-android-application)

* What is obfuscation? What is it used for? What about minification?

* How do you build your apps for release?

* How do you control the application version update to specific number of users?

* Can we identify users who have uninstalled our application?

* Implement Search Using RxJava Operators. [MindOrks](https://blog.mindorks.com/implement-search-using-rxjava-operators-c8882b64fe1d)

* APK Size Reduction. [MindOrks](https://blog.mindorks.com/how-to-reduce-apk-size-in-android-2f3713d2d662)

* Android Development Best Practices. [MindOrks](https://blog.mindorks.com/android-development-best-practices-83c94b027fd3)

* Android Code Style And Guidelines. [MindOrks](https://blog.mindorks.com/android-code-style-and-guidelines-d5f80453d5c7)

* Have you tried Kotlin? [MindOrks](https://blog.mindorks.com/why-you-must-try-kotlin-for-android-development-e14d00c8084b)

* What are Coroutines in Kotlin? [MindOrks](https://blog.mindorks.com/mastering-kotlin-coroutines-in-android-step-by-step-guide)

* What are the metrics that you should measure continuously while android application development? [MindOrks](https://blog.mindorks.com/android-app-performance-metrics-a1176334186e)

* What is Chrome Custom Tabs? How to display web content in your app? [MindOrks](https://blog.mindorks.com/android-browser-lets-launch-chrome-custom-tabs-with-kotlin)

### Background Processing

 * [Raywenderlich](https://www.raywenderlich.com/5306-android-background-processing)
 * [AndroidPub](https://android.jlelse.eu/8-ways-to-do-asynchronous-processing-in-android-and-counting-f634dc6fae4e)
 * [Journaldev](https://www.journaldev.com/9708/android-asynctask-example-tutorial)
 * [Vogella](https://www.vogella.com/tutorials/AndroidBackgroundProcessing/article.html)


### Collection

* [10 Android interview question answers for Freshers](http://www.careerride.com/android-interview-questions.aspx)
* [20 Essential Android Interview Questions from Toptal](http://www.toptal.com/android/interview-questions)
* [50 android interview questions & answers](http://career.guru99.com/50-android-interview-questions-answers/).
* [A couple of Android questions posted by Quora users](https://www.quora.com/What-are-good-job-interview-questions-for-an-Android-developer)
* [A great list of Android interview questions covering all the aspects of this career](http://www.tutorialspoint.com/android/android_interview_questions.htm)
* [Collection of Android and Java related questions and topics, including general developer questions, Java core, Data structures, Build Tools, Programming Paradigms, Core Android, Databases and etc](https://github.com/derekargueta/Android-Interview-Questions)
* [Collection of Android and Java questions divided by experience](https://medium.com/@neteinstein/not-another-android-interviews-article-the-questions-3dedafa30bec)
* [Android Interview Questions & How to Interview Candidates](https://pangara.com/blog/android-interview-questions)
