# Ionic_interview_questions
Interview Questions for ionic (1, 2 ,3 and 4)

# 1. What is Ionic ?


      Ionic is a mobile app development framework used to build hybrid apps. Hybrid apps are basically web apps running in a browser within a wrapper that  has access to the native platform layer. Ionic framework is an HTML5 framework. It needs a native wrapper like Cordova or PhoneGap in order to run as a native app. Ionic framework lets you maintain one codebase and create builds for both Android and iOS platforms.

    NodeJS , npm are required in order to install Ionic. You need NodeJS 6.0.0+ or a higher version in order to install ionic. 
    
# 2. Who Developed Ionic Framework ?

Ionic Framework was created by Drifty Co. in 2013 and developed by Max Lynch, Ben Sperry, and Adam Bradley.

# 3. What is AOT and JIT. Which is used by ionic ?


  Since Ionic (1, 2, 3 and 4) are majorly dependent on Angular. The Compilation options that were available for Angular were available for Ionic too. I have mentioned them below.

JIT stands for Just in Time compiler. It is a type of compilation where a compilation of the app happens in the browser at runtime.

AOT stands for ahead of time compiler. It is a type of compilation that compiles the app at build time.

If we just use ionic cordova build platform (android or ios) then it will be JIT if we use prod flag I, E ionic cordova build platform --prod then it will use AOT.

An app that is built with JIT is slow as compared to AOT. But compilation time required for AOT is more than JIT. So for a quick checks use JIT and for a final deployment use AOT.

# 4. How to debug ionic app in real device( Android and iOS )


   In Ionic We can debug Android and iOS apps on Chrome or Safari Browser.

   Android: To debug an Android app in real time, we need to follow below steps.
   
    1. Enable developer mode on Android Mobile.
    
    2. Run the app on the real device either by running ionic Cordova run android or build the apk by running ionic Cordova build android and transfer it to the phone.
    
    3. Connect device to your computer with a USB cable and lunch Google Chrome browser and open URL chrome://inspect/#devices which will display your phone and app name. Click on inspect there.
    
    4. Now you will be able to inspect the app and check the logs.
    
  iOS: To debug the iOS app in real-time, we need to follow below steps
  
    1. Run the app on the device by executing command ionic Cordova run-ios or build the app with ionic Cordova build ios and Xcode to   launch the app on the phone.
    
    2. Now open safari browser -> windows -> Enable developer options.
    
    3. Now open developer -> Your phone -> localhost, now you will be able to debug the app in real-time.

# 5. What is difference between Phonegap , Cordova and Ionic ?

      # PhoneGap: PhoneGap is a framework developed by Adobe Systems. It is used for developing mobile applications and can be used by anyone with the knowledge of CSS, HTML, JScript. PhoneGap is a propitiatory version of Apache Cordova and gives extra features apart from the existing Cordova.
      
      
      # Cordova: Cordova is a JavaScript framework which builds apps, which can access the device hardware. Cordova cannot build UI interactions of mobile apps because it uses HTML5, CSS6, Sencha to build UI. However, it supports other web technologies used to develop mobile apps. Cordova is also known as Apache Cordova.
      
      
      # Ionic: Ionic framework is a set of CSS, JVscript library, built on Cordova and AngularJS
 
 # 6. How can you render a 5000 item list in Ionic, without affecting scroll performance?
 
 Ionic provides a collection-repeat directive that renders only visible items in the DOM. So even if the list is huge, like 5000 in our example, only items visible in a viewport are rendered. Thus, scroll performance is not affected.

# 7. What’s the difference between “ionic build” and “ionic prepare”?

ionic prepare <platform> copies all files from the www folder into the target platform’s www folder.

ionic build <platform> also does this, but also builds the app’s source code so that it can be run on a simulator/emulator or a device.
      
# 8. how do you deploy an Ionic project onto a device?

To deploy your app in device, all you have to do is enable USB Debugging and Developer Mode on your Android device, then run ionic cordova run android --device from the command line.

# 9. How to update Cordova plugins ?

Use the following command to update Cordova plugins.

npm install -g cordova-check-plugins
cordova-check-plugins --update=auto

# 10. What is Web View in Ionic ?

Web Views are full screen web browser which iss capable to render apps made with web technologies like HTML, Javascript, css. Ionic uses web technologies to create hybrid mobile apps.

# 11. What's New in Ionic 4 ?

Ionic 4 comes with following outstanding Features that make cross-app development more easy and comfortable.

      -> Web Components
      -> Capacitor
      -> Stencil (web component compiler)
      -> ion-Backdrop (Full-screen components which overlay other components)
      -> ion-Picker
      -> ion-Ripple Effect
      -> ion-Route
      -> Color Changes
      -> Lazy Loading
      -> CSS Variables
      -> Ionic Native 5
# 12. What are the benefits of caching views in Ionic applications?

In Ionic, caching of up to ten views is done by default. This improves performance and assists in maintaining different states simultaneously in the views. For instance, cache maintains scroll position in the views or the active state of buttons.

# 13. What is Ionic Native?

It is a Typescript wrapper for PhoneGap/Cordova plugins. Its purpose is to ease the process of adding native functionalities to your Ionic app.



