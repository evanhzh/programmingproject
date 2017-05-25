---
layout: post
title: How to start Xcode project without Storyboard
description: Developing iOS app programmatically
image: assets/images/blog-img/galymzhan-abdugalimov-181-min.jpg
medium: https://medium.com/@evanzhoe/summarizing-how-to-start-xcode-project-programmatically-ecab6d2a977a
---
![pic-01](/assets/images/blog-img/Start-XCode-Without-Storyboard/pic-01.png)

I have just completed LetsBuiltThatApp Basic Training Course developed by Brian Voong on how to build a custom simple Kindle app without the help of storyboard.  
It is a totally different experience to start my Xcode project by setting up a new ViewController using a custom name and then removing the storyboard!


Today, my challenge is to set up a new Xcode project so that I can work on an iOS application development programmatically. Thanks to Brian, now I know what I should do to get myself all set for that. Although there are quite some steps to get our project set up, most of his approach is to keep running the simulator after a few lines and build on from the error displayed on the console.
So, today, I would like to challenge myself to put together a summary that would help me start any project on Xcode in a breeze.

**To get started:**
1. Create a new Swift file in your workspace folder. (This file would be your custom ViewController replacing the default ViewController)
 * Import UIKit to have access to ViewController class.  
 * Create a new class.  
 * In that class, create a function to override the viewDidLoad.
 ![pic-01](/assets/images/blog-img/Start-XCode-Without-Storyboard/pic-01.png)

2. Select your AppDelegate file. Notice the variable window: UIWindow? is already declared in your AppDelegate file? Now, in the application function, type:    
 * window = UIWindow(frame: UIScreen.main.bounds)  
 * window?.makeKeyAndVisible()




3. Now, create a new variable to store the instance of custom ViewController class with a collectionViewLayout parameter:  
 * UICollectionViewFlowLayout is the layout design that we want to use if you intend to create columns or rows of cells. Think of your Twitter app homepage. Here’s the definition from the documentation:
 >The `UICollectionViewFlowLayout` class is a concrete layout object that organizes items into a grid with optional header and footer views for each section. The items in the collection view flow from one row or column (depending on the scrolling direction) to the next, with each row comprising as many cells as will fit. Cells can be the same sizes or different sizes.

4. Finally, assign UINavigationController with the rootViewController parameter.
![ViewController2](/assets/images/blog-img/Start-XCode-Without-Storyboard/pic-02.png)

  We want to put our custom ViewController in the spotlight when running the simulator. We can do that by specifying it to our rootViewController.

  Here’s the explanation from the Apple’s documentation:

  > The root view controller provides the content view of the window. Assigning a view controller to this property (either programmatically or using Interface Builder) installs the view controller’s view as the content view of the window.*

We are all set!

You can now remove your Storyboard from your workspace. It’s a bit daunting to move the Storyboard to trash at first, but I’m already getting used to it. Don’t forget to clear out the Main Interface to avoid error. By default, it holds a reference to the Storyboard.
