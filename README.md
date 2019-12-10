# Ionic_interview_questions
Interview Questions for ionic (1, 2 ,3 and 4)

# 1. What is Ionic ?


      Ionic is a mobile app development framework used to build hybrid apps. Hybrid apps are basically web apps running in a browser within a wrapper that  has access to the native platform layer. Ionic framework is an HTML5 framework. It needs a native wrapper like Cordova or PhoneGap in order to run as a native app. Ionic framework lets you maintain one codebase and create builds for both Android and iOS platforms.

    NodeJS , npm are required in order to install Ionic. You need NodeJS 6.0.0+ or a higher version in order to install ionic. 

# 2. What is AOT and JIT. Which is used by ionic ?


  Since Ionic (1, 2, 3 and 4) are majorly dependent on Angular. The Compilation options that were available for Angular were available for Ionic too. I have mentioned them below.

JIT stands for Just in Time compiler. It is a type of compilation where a compilation of the app happens in the browser at runtime.

AOT stands for ahead of time compiler. It is a type of compilation that compiles the app at build time.

If we just use ionic cordova build platform (android or ios) then it will be JIT if we use prod flag I, E ionic cordova build platform --prod then it will use AOT.

An app that is built with JIT is slow as compared to AOT. But compilation time required for AOT is more than JIT. So for a quick checks use JIT and for a final deployment use AOT.

# 3. How to debug ionic app in real device( Android and iOS )


   In Ionic We can debug Android and iOS apps on Chrome or Safari Browser.

   Android: To debug an Android app in real time, we need to follow below steps.
   
    1. Enable developer mode on Android Mobile.
    
    2. Run the app on the real device either by running ionic Cordova run android or build the apk by running ionic Cordova build        android and transfer it to the phone.
    
    3. Connect device to your computer with a USB cable and lunch Google Chrome browser and open URL chrome://inspect/#devices which    will display your phone and app name. Click on inspect there.
    
    4. Now you will be able to inspect the app and check the logs.
    
  iOS: To debug the iOS app in real-time, we need to follow below steps
  
    1. Run the app on the device by executing command ionic Cordova run-ios or build the app with ionic Cordova build ios and Xcode to   launch the app on the phone.
    
    2. Now open safari browser -> windows -> Enable developer options.
    
    3. Now open developer -> Your phone -> localhost, now you will be able to debug the app in real-time.
