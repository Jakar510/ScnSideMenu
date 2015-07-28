ScnSideMenu
======================
Xamarin.Forms side menu control (targeted at Android, iOS and Windows Phone)

Description of control
===========================================
Control suggests use two panel side bar on your choosing: left or right panel or two panel together. For that need to set necessary flag in constructor.
You can call through changing property IsShowLeftPanel/IsShowRightPanel or use swipe gesture near border.
For hiding panel use also changing property or swipe gesture on panel.

Screenshots
===========================================
All screenshots are made on Android platform, but in other platforms they looks the same.
Bellow is shown schematic representation without any stylizing.
![Main](Screenshots/Droid/SideMenuSample.png)

Bellow is shown screenshots from real application.
You can find sources of this application here: https://github.com/ScienceSoft-Inc/XamarinDiscountsApp.
![Main](Screenshots/Droid/SideMenuRealApp.png)

How to use this control in Xamarin.Forms app
===========================================
Look sample to know how right include control menu in your application.

If you want to use custom gestures for closing SideMenu then need to add initialize renderers for each platform.

In iOS project just use
```cs
Xamarin.Forms.Forms.Init ();
ViewGesturesRenderer.Init();
```
In Android project just use
```cs
Xamarin.Forms.Forms.Init (this, bundle);
ViewGesturesRenderer.Init();
```
In WinPhone project just use
```cs
Xamarin.Forms.Forms.Init ();
ViewGesturesRenderer.Init();
```