# Android_app

simple project 
<h3>XML FOR ANDROID </h3>
<h5> Vector drawables overview </h5>

Android Studio can also convert SVG/PSD files to the vector drawable format<br>
The major advantage of using a vector drawable is image scalability. It can be scaled without loss of display quality, which means the same file is resized for different screen densities without loss of image quality. This results in smaller APK files and less developer maintenance


```diff
+  Right click on app folder-> New Vector Asset.
+  Select second option in radio button to create vector from local file as shown in below image.
```

for more doc see this <a href="https://developer.android.com/guide/topics/graphics/vector-drawable-resources" target="_blank">link</a> <br>
<br>
<h5>fitsSystemWindows= true</h5>
When people want to put some View under status bar they usually can find the answer like:


```diff
-  “Just add “fitsSystemWindows= true” and it should work fine. -No? 
-  Then change your root view to CoordinatorLayout and apply fitsSystemWindows = true”.
```

<img src="./image_githubDoc/1_MTnHZLNhcO9RaC948i53vw.png"><br>
for more docs see this <a href="https://proandroiddev.com/draw-under-status-bar-like-a-pro-db38cfff2870" target="_blank">link1 </a>, <a href="https://medium.com/androiddevelopers/why-would-i-want-to-fitssystemwindows-4e26d9ce1eec" target="_blank">link2</a><br>

<h5>tools:openDrawer="start"</h5>
If I remove the tools:openDrawer="start", on the layout preview, the navigation drawer will be closed instead of open.<br>
I thought this was a replacement attribute, similar to android:text that can be replaced with tools:text to put some placeholder text in the layout preview.<br>

<h5>Android ScrollView Vs ListView</h5>
ListView is meant to create a list of varrying lengths based of an array of information. ScrollView is for having a (usually) set amount of children in the View (defined in the layout xml).<br>

ListViews do not inflate all items, they inflate however many can fit on a page at a time. Your fastest option, with or without paging is a ListView. However, if each child is completeley different, then ScrollView is the way to go.<br>

fillViewport = “true”
fillViewport allows scrollView to extend it’s height equals to the full height of device screen’s height in the cases when the child of scroll view has less height.
see this doc <a href"https://demonuts.com/android-fillviewport/" target="_blank">link</a>
