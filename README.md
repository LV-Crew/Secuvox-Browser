# Secuvox-Browser
A Firefox based browser aiming at privacy

1.) Fingerprinting
    Plugins nicht zurückgeben ausser Flash, Silverlight, Java <- ändern in fake
    /dom/base/Navigator.cpp
    /dom/base/nsPluginArray.cpp

2.) mouseover / mouseenter / mouseleave: method not implemented zurückgeben
    /dom/base/nsINode.cpp
    /dom/events/EventListenerManager.cpp
    /dom/events/JSEventHandler.cpp

3.) Fingerprinting 
    Screen size definiert zurückgeben
    /dom/base/nsScreen.cpp

4.) Fingerprinting
    Canvas
    /dom/canvas/CanvasRenderingContext2D.cpp
    /dom/html/HTMLCanvasElement.cpp

5.) Fingerprinting
    Keine fonts zurückgeben
    /layout/style/FontFaceSet.cpp

6.) Adblocker
    /netwerk/dns/GetAddrInfo.cpp
