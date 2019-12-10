# ionic_interview_questions
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
