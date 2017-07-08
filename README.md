# Secuvox-Browser
A Firefox based browser aiming at privacy<br>
<br>
1.) Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Plugins nicht zurückgeben ausser Flash, Silverlight, Java <- Ändern in fake<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/Navigator.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsPluginArray.cpp<br>
<br>
2.) mouseover / mouseenter / mouseleave: method not implemented zurückgeben<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsINode.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/events/EventListenerManager.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/events/JSEventHandler.cpp<br>
<br>
3.) Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Screen size definiert zurückgeben<br>
&#160;&#160;&#160;&#160;&#160;/dom/base/nsScreen.cpp<br>
<br>
4.) Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Canvas<br>
&#160;&#160;&#160;&#160;&#160;/dom/canvas/CanvasRenderingContext2D.cpp<br>
&#160;&#160;&#160;&#160;&#160;/dom/html/HTMLCanvasElement.cpp<br>
<br>
5.) Fingerprinting<br>
&#160;&#160;&#160;&#160;&#160;Keine fonts zurückgeben<br>
&#160;&#160;&#160;&#160;&#160;/layout/style/FontFaceSet.cpp<br>
<br>
6.) Adblocker<br>
&#160;&#160;&#160;&#160;&#160;/netwerk/dns/GetAddrInfo.cpp<br>
<br>
<br>
http://www.secuvox-browser.com<br>
