# Secuvox-Browser
A Firefox based browser aiming at privacy<br>
<br>
Features:<br>
- Hide Plugins-Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Plugins nicht zurückgeben ausser: Flash, Silverlight, Java<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/Navigator.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsPluginArray.cpp<br>
- Hide Mouse-Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Method not implemented zurückgeben for: mouseover / mouseenter / mouseleave<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsINode.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/events/EventListenerManager.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/events/JSEventHandler.cpp<br>
- Hide Screen-Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Screen size definiert zurückgeben<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsScreen.cpp<br>
- Hide Canvas-Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Canvas<br>
&#160;&#160;&#160;&#160;&#160;/dom/canvas/CanvasRenderingContext2D.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/html/HTMLCanvasElement.cpp<br>
- Hide Fonts-Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Keine fonts zurückgeben<br>
&#160;&#160;&#160;&#160;&#160;/layout/style/FontFaceSet.cpp<br>
- Adblocker<br>
&#160;&#160;&#160;&#160;&#160;Adblocker based on a hosts-file<br>
&#160;&#160;&#160;&#160;&#160;/netwerk/dns/GetAddrInfo.cpp<br>
<br>
<br>
To-dos:<br>
- Hide plugins Flash, Silverlight, Java<br>
<br>
<br>
Homepage-URL: http://www.Secuvox-Browser.com<br>
