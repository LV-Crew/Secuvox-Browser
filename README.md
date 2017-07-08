# Secuvox-Browser
A Firefox based browser aiming at privacy<br>
<br>
1.) Fingerprinting<br>
    Plugins nicht zurückgeben ausser Flash, Silverlight, Java <- ändern in fake<br>
    /dom/base/Navigator.cpp<br>
    /dom/base/nsPluginArray.cpp<br>
<br>
2.) mouseover / mouseenter / mouseleave: method not implemented zurückgeben<br>
    /dom/base/nsINode.cpp<br>
    /dom/events/EventListenerManager.cpp<br>
    /dom/events/JSEventHandler.cpp<br>
<br>
3.) Fingerprinting<br>
    Screen size definiert zurückgeben<br>
    /dom/base/nsScreen.cpp<br>
<br>
4.) Fingerprinting<br>
    Canvas<br>
    /dom/canvas/CanvasRenderingContext2D.cpp<br>
    /dom/html/HTMLCanvasElement.cpp<br>
<br>
5.) Fingerprinting<br>
    Keine fonts zurückgeben<br>
    /layout/style/FontFaceSet.cpp<br>
<br>
6.) Adblocker<br>
    /netwerk/dns/GetAddrInfo.cpp<br>
