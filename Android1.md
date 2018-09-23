## Android 1
### Presenter: Joanna Chen

**Target Audience:** 
- Hackers who are unfamiliar with the Android development environment

**Suggested Prerequisites:** 
- A basic understanding of programming fundamentals 
- Downloading Android Studio
 
**Workshop Goals:**
- Create a basic Android app Activity. 
 
**Description:**

Get acquainted with Android development and make those first steps towards creating an app. In this workshop, you will: 
- Become familiar with the Android Studio environment 
- Understand the purpose of the Layout, Java, and manifest files
- Understand basic XML
- Understand how to give functionality to front-end elements

**Content Breakdown:**
- Creating a new project and explaining the different buttons in Android Studio
- Explaining the basics of an Android app: structure, layouts (XML), UI elements 
- Creating UI elements: ImageViews, TextViews, Buttons in XML
- Adding code to make an interactive button that will change UI elements
- Q&A

**[Slides](https://docs.google.com/presentation/d/1y4i5Xp9gnhDlRnCHXAHhfjvx3MKwnh3D48TEhDL8soY/edit?usp=sharing)**

--- 

**Key Notes:** 
* XML structure: 
    * Tags indicate the structure (eg. \<LinearLayout\> … \</LinearLayout\>, \<TextView … /\>)
    * Various attributes can also be set inside of the tags (eg. android:Text = “Hello”) 

* Linear layout: 
    * Can have vertical or horizontal orientation
    * The order in which you put the XML blocks is the order in which the elements appear

* Views/UI Elements
    * Must indicate width and height (either match_parent, wrap_content, or fixed value) 
    * ImageViews: can set the src to be an image that you include in the app files
    * TextViews: can set text, font family, textSize, etc. 
    * Buttons: can set clickable, text, background
          * In the Java file, you can attach an onClickListener(..) to allow for user interaction
