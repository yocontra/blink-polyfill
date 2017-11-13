blink-polyfill
==============

Blinking has been a staple of innovation since the dawn of human culture and now they are trying to take it away.

## Timeline

- __1994:__ Papa Netscape releases 1.0 with the blink tag
- __1994-2013:__ The internet thrives in its blinking glory
- __2012-2013:__ Opera, Chrome, IE, and Firefox completely remove the blink tag. The web weeps.

## The Outrage

OaklawnM4M:
> I really hate companies that brag about how compliant they are when in reality they don't give a damn whether you like their offerings or not. I'm so looking forward to the release of IE version  9 made by the same company that makes the operating system for the computer that it's running on.
> When it comes to HTML, the programmer isn't supposed to pick and choose what they want to support/comply with cuz if they do then standards are no longer standard.  PERIOD
> And don't try to use the excuse of "Well it's FREE and you didn't pay for it"  cuz that dog don't hunt either.  All the ajax and java in the world isn't an excuse to eliminate a feature that's 25 years old.  But while we're at it, why don't we start eliminating words from the dictionary too..  Let's start with the word "screwed" so nobody will know that it's being done to them..  Or how about "incompetent" then nobody will ever know what an idiot you are.

somebodystolefatboy:
> Well, you \<blink\> haters might be singing a different tune if you had Ebay morons giving you negative  feedback because they cannot or will not actually read the item description. \<blink on!\>

drewying:
> Fare well old \<blink\> friend. My high school memories of webrings would not be the same without you.

## The Fix

Don't let these "standards" punks steal the web. Place this CSS on your page today.

```css
@-moz-keyframes blink {
 0% {
   opacity: 1;
 }
 50% {
   opacity: 0;
 }
 100% {
   opacity: 1;
 }

}

@-webkit-keyframes blink {
 0% {
   opacity: 1;
 }
 50% {
   opacity: 0;
 }
 100% {
   opacity: 1;
 }

}

@-o-keyframes blink {
 0% {
   opacity: 1;
 }
 50% {
   opacity: 0;
 }
 100% {
   opacity: 1;
 }

}

@keyframes blink {
 0% {
    opacity: 1;
 }
 50% {
    opacity: 0;
 }
 100% {
    opacity: 1;
 }
}

blink {
  -webkit-animation: blink 1s steps(1) infinite;
  -moz-animation: blink 1s steps(1) infinite;
  -o-animation: blink 1s steps(1) infinite;
  animation: blink 1s steps(1) infinite;
}
```

