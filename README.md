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


# 14. Difference between Ionic 4 and Ionic 3

 # Changes in Package Name
In Ionic 4, the package name starts with @ symbol like @ionic/angular. Whereas, the Ionic 3 package name does not use the @ symbol. We can understand the syntax comparison of Ionic 3 and ionic 4 from the below syntax.

In Ionic 3: npm install ionic-angular  
In Ionic 4: npm install @ionic/angular  

If you are going to migrating an app from Ionic 3 to Ionic 4, you need to update the imports from ionic-angular to @ionic/angular.

# 15. The List of Useful Ionic Framework Commands?
The commands and its description
1.          start- This command is used to create a new project
2.          generate-  This command is used to generate pipes, components, pages, directives, providers and tabs
3.          serve- This command is used to start a local dev server for app dev/testing
4.          build - This command is used to Build web assets and prepare your app for any platform targets
5.          docs - This command is used to Open the Ionic documentation website
6.          info - This command is used to Print system/environment info
7.          link- This command is used to Connect your local app to Ionic
8.          login- This command is used to Login with your Ionic ID
9.          signup - This command is used to Create an Ionic account
10.     telemetry-  This command is used to Opt in and out of telemetry
11.     upload- This command is used to Upload a new snapshot of your app
12.     config get- This command is used to Print config values
13.     config set- This command is used to Set config values
14.     cordova build- This command is used to Build an Ionic project for a given platform
15.     cordova compile- This command is used to compile native platform code
16.     cordova emulate- This command is used to Emulate an Ionic project on a simulator or emulator
17.     cordova platform- This command is used to Manage Cordova platform targets
18.     cordova plugin - This command is used to Manage Cordova plug-in
19.     cordova prepare - This command is used to Copies assets to Cordova platforms, preparing them for native builds
20.     cordova resources - This command is used to Automatically create icon and splash screen resources
21.     package build- This command is used to Start a package build
22.     package download- This command is used to Download your packaged app
23.     package list - This command is used to List your cloud builds
24.     package info - This command is used to Get info about a build
25.     cordova run - This command is used to Run an Ionic project on a connected device


# 16. What Are the Others Ionic Commands also Available for Angular?

Ionic Commands also Available for Angular Projects -
1.          Pipes,
2.          Components,
3.          Directives,
4.          Providers and
5.          Tabs
6.          And So On
Syntax –
1.          ionic generate [<pipes>] [<pipes-name>]
2.          ionic generate [<components>] [<components-name>]
3.          ionic generate [<directives>] [<directives-name>]
4.          ionic generate [<providers>] [<providers-name>]
5.          ionic generate [<tabs>] [<tabs-name>]
      
      
# 17. How to parse JSON in Ionic Framework?

he JSON.parse() method parses a JSON string, constructing the JavaScript value or object described by the string.
The Example is -
var users = JSON.parse(userResponseData);

# 18. How To Disable / Enable Content Scrolling in IONIC Framework?
We can disable/enable scrollbar pragmatically.

Example 1 -  
Try a setting <content scroll="false"> that will disable scrolling.

Example 2-
You can also use this as a quick fix –

This every time an event is called, in our case, on every drag event.
 
Disable Scrolling -
$ionicScrollDelegate.getScrollView().__enableScrollY = false


Enable Scrolling -
$ionicScrollDelegate.getScrollView().__enableScrollY = true


Example 3,
$timeout(function(){
   $ionicScrollDelegate.$getByHandle('formularContent').freezeScroll(true);
})

Example 4,
Add the .scss file –
.no-scroll .scroll-content{
    overflow: hidden;
}

And
Then add the no-scroll class to your ion-content like this –
<ion-content class="no-scroll">
</ion-content>
