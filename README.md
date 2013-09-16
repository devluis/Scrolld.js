Scrolld.js
==========
README

1. About
2. Use
3. Tweaks
4. Demo
5. Download
6. License

// ABOUT //

Scrolld.js is a unique open source plugin for jQuery.
Scrolld.js provides a method for highly precise scrolling for pixel-perfect layouts and navigation using real-time updated data values.
With Scrolld.js your scrolling to items will always be exact and will always provide the best user experience.
Scrolld.js is specifically designed to support responsive designs and turns navigating long pages into a simple task.
Scrolld.js is intended for easy use and is fully deployable within minutes.

* Scrolld.js is simple and works with just an element id tag. *

// HOW TO USE //

1 | Download the source & upload it to your server.

2 | Place the script include file on your page: 

Ex:

 ```<script type="text/javascript" src="../js/scrolld.js"></script> ```

3 | Place this trigger script at bottom of body:

Ex:

```
<script type="text/javascript">
$("[id*='Btn']").stop(true).on('click',function(e){e.preventDefault();$(this).scrolld();})
</script>
```

4 | Use specific id tags to control scrolling, one for the anchor & one for the target.
Anchor id must be in the format of *Btn and target id must be *.

Ex:
```<a id='useBtn' class='*' href='*'>```
```<div id='use' class='*'>```

5 | Keep the defaults or easily tweak the settings for a custom fit.

// TWEAKS //

Scrolld.js was built with quick and simple customization in mind. You can easily customize the entire experience with these few parameters. 

```
* Head to the defaults section of the scrolld.js / scrolld.min.js file *

Web Settings: 

var scrolldDistance = scrolldPre;
var scrolldDistanceMin = scrolldPre;
var scrolldCustom = 0;
var scrolldSpeed = speed11;
var scrolldEasing = 'scrolldEasing1';
var scrolldFixed = true;
var scrolldNavBar = fixedNavBar; 

Mobile Settings:

var scrolldMobile = true;
var scrolldMobileWidth = 979;
var scrolldMobileDistance = scrolldPre;
var scrolldMobileDistanceMin = scrolldPre;
var scrolldMobileSpeed = speed11;
var scrolldMobileEasing = 'scrolldEasing1';
var scrolldMobileFixed = true;
var scrolldMobileNavBar = fixedNavBar;
```
Targeting A Single Div Easing - Web, Or Mobile, Or Both:

Simply give the anchor a class name of the desired easing method, include Mobile at the end of the class to target only mobile, include both to target both.

Ex:
```<a id='useBtn' class='easeOutBounce easeOutBounceMobile' href='*'>```


// DETAILED SETTINGS INFORMATION


```scrolldDistance``` - Set scroll distance from target div: 
```
scrolldPre* = Scrolls to the exact top of div less dynamic value based on window height
scrolldTop = Scrolls to the exact top of div ( less nav bar height if set )
scrolldCenter = Scrolls to div in the exact center of browser window
```

```scrolldDistanceMin``` - Set scroll distance from target div if div is larger than current window size: 
```
scrolldPre* = Scrolls to the exact top of div less dynamic value based on window height
scrolldTop = Scrolls to the exact top of div  ( less nav bar height if set )
scrolldCenter = Scrolls to div in the exact center of browser window
```

```scrolldCustom``` - Set additonal +- distance from target div (for top & pre settings only): 

```
*scrolldCustom is separate from the other parameters*
*It is located at the very top of the scrolld.js/scrolld.min.js file.*

scrolldCustom = 0*
```

```scrolldSpeed``` - Set scroll speed to target; 
Scrolls to div in x miliseconds, set a number value or use a preset variable:
```
Preset Scroll Speed Settings:

var speed1 = 100;
var speed2 = 200;
var speed3 = 300;
var speed4 = 400;
var speed5 = 500;
var speed6 = 600;
var speed7 = 700;
var speed8 = 800;
var speed9 = 900;
var speed10 = 1000;
var speed11* = 1100;
var speed12 = 1200;
var speed13 = 1300;
var speed14 = 1400;
var speed15 = 1500;
var speed16 = 1600;
var speed17 = 1700;
var speed18 = 1800;
var speed19 = 1900;
var speed20 = 2000;
var speedX = 1234; // Set Custom Speed Setting Here
```

scrolldEasing - Set scroll easing function type; Options include all jQuery preset + new custom easing functions: 

jQuery Preset Easings:

```
*Visit Easings.net for current jQuery easing presets in action.*

linear
swing
jswing
easeInQuad
easeOutQuad
easeInOutQuad
easeInCubic
easeOutCubic
easeInOutCubic
easeInQuart
easeOutQuart
easeInOutQuart
easeInQuint
easeOutQuint
easeInOutQuint
easeInSine
easeOutSine
easeInOutSine
easeInExpo
easeOutExpo
easeInOutExpo
easeInCirc
easeOutCirc
easeInOutCirc
easeInElastic
easeOutElastic
easeInOutElastic
easeInBack
easeOutBack
easeInOutBack
easeInBounce
easeOutBounce
easeInOutBounce
``` 
Custom Easings - New unique easing methods personally developed for Scrolld.js
```
scrolldEasing1*
scrolldEasing2
scrolldEasing3
```

scrolldFixed - Set boolean if you use a fixed website header: 

```var scrolldFixed = true*; ```

Note: If you use a fixed header, you must also define the id for the header div: 

```scrolldMobileNavBar = fixedNavBar```

Scrolld Mobile Specific Settings:
```
scrolldMobile - Set boolean if your website uses a responsive mobile layout. 
scrolldMobileWidth - Define the max width used for mobile devices to trigger mobile functions. 
scrolldMobileDistance - Set scroll distance from target div. 
scrolldMobileDistanceMin - Set scroll distance from target div if div is larger than current window size. 
scrolldMobileSpeed - Set scroll speed to target used only with mobile devices. 
scrolldMobileEasing - Set scroll easing function used only with mobile devices. 
scrolldMobileFixed - Set boolean if your mobile layout uses a fixed header.
```

```* Indicates default values.```

// DEMO //

Visit www.scrolldjs.com/demo.php for multiple demos.

// DOWNLOAD //

Visit the Scrolld.js GitHub repository for download link.

// LICENSE //

(MIT License)

Copyright (C) 2013 Charles Geiger

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
