blink-polyfill
==============

Blinking has been a staple of innovation since the dawn of human culture and now they are trying to take it away.

## Timeline

- 1994: Papa Netscape releases 1.0 with the blink tag
- 1994-2013: The internet thrives in it's blinking glory
- 2013: Opera, Chrome, and Firefox completely remove the blink tag. The web weeps.

## The Outrage

> I really hate companies that brag about how compliant they are when in reality they don't give a damn whether you like their offerings or not. I'm so looking forward to the release of IE version  9 made by the same company that makes the operating system for the computer that it's running on. 
> When it comes to HTML, the programmer isn't supposed to pick and choose what they want to support/comply with cuz if they do then standards are no longer standard.  PERIOD   
> And don't try to use the excuse of "Well it's FREE and you didn't pay for it"  cuz that dog don't hunt either.  All the ajax and java in the world isn't an excuse to eliminate a feature that's 25 years old.  But while we're at it, why don't we start eliminating words from the dictionary too..  Let's start with the word "screwed" so nobody will know that it's being done to them..  Or how about "incompetent" then nobody will ever know what an idiot you are.

## The Fix

Place this CSS on your page. All of your problems will be solved.

```css
@keyframes "blink" {
 0% {
    -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
     filter: alpha(opacity=100);
   	opacity: 1.0;
 }
 50% {
    -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
   	filter: alpha(opacity=0);
   	opacity: 0.0;
 }
 100% {
    -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
   	filter: alpha(opacity=100);
   	opacity: 1.0;
 }

}

@-moz-keyframes blink {
 0% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }
 50% {
   filter: alpha(opacity=0);
   opacity: 0.0;
 }
 100% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }

}

@-webkit-keyframes "blink" {
 0% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }
 50% {
   filter: alpha(opacity=0);
   opacity: 0.0;
 }
 100% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }

}

@-ms-keyframes "blink" {
 0% {
   -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
   filter: alpha(opacity=100);
   opacity: 1.0;
 }
 50% {
   -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
   filter: alpha(opacity=0);
   opacity: 0.0;
 }
 100% {
   -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
   filter: alpha(opacity=100);
   opacity: 1.0;
 }

}

@-o-keyframes "blink" {
 0% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }
 50% {
   filter: alpha(opacity=0);
   opacity: 0.0;
 }
 100% {
   filter: alpha(opacity=100);
   opacity: 1.0;
 }

}

blink {
	-webkit-animation-name: blink;
	-moz-animation-name: blink;
	-ms-animation-name: blink;
	-o-animation-name: blink;
	animation-name: blink;

	-webkit-animation-iteration-count: infinite;
	-moz-animation-iteration-count: infinite;
	-ms-animation-iteration-count: infinite;
	-o-animation-iteration-count: infinite;
	animation-iteration-count: infinite;

	-webkit-animation-timing-function: steps(1);
	-moz-animation-timing-function: steps(1);
	-ms-animation-timing-function: steps(1);
	-o-animation-timing-function: steps(1);
	animation-timing-function: steps(1);
	-webkit-animation-duration: 1s;
}
```
