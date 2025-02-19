---
draft: true
---
Zen browser is to Firefox what Arc browser is to chrome. It is a Browser that is an open source project mainly maintained by one person. I have been using Zen for the past 4 months and it has been a really nice experience. I am not a full fledged power use but neither am I a complete noob user. The tab management and the customization has to be one of the nicest out there while even the out of box experience is extremely intuitive and usable!

While using Zen I love that it syncs my browser data with my Mozilla account. To enhance this experience I was wondering if there could be a phone implementation of Zen, not as a full fledged browser but to optimize and reduce friction while switching between Mobile browsing and desktop. here are some initial thoughts-

- Normally never use Mobile browsing for intensive research.
- when I am in researching on my phone I always send the tabs to my desktop to get back to it later.
- my major mobile use cases are 
	- opening links from apps
	- filling forms
	- reading articles
	- downloading content for phone, images, gifs, music
- things I struggle to do
	- share media to phone
	- continue browsing in desktop(in case I forgot to send the tabs to my desktop)

here are some design proposals for Zen as a mobile app

Zen mobile must be a companion rather than a full fledged browsing app
- Lots of browsers try to give the full browsing experience to mobile but fail to do so
- the reality is that mobile browsing and desktop browsing are completely different!


`/* CSS HEX */ 
--myrtle-green: #407376ff; 
--pear: #CED02Fff;
--glaucous: #757CB4ff; 
--lemon-chiffon: #E0E2B8ff; 
--picton-blue: #19A1D9ff; 
/* CSS HSL */ 
--myrtle-green: hsla(183, 30%, 36%, 1); 
--pear: hsla(61, 63%, 50%, 1); 
--glaucous: hsla(233, 30%, 58%, 1); 
--lemon-chiffon: hsla(63, 42%, 80%, 1); 
--picton-blue: hsla(197, 79%, 47%, 1); 
/* SCSS HEX */ 
$myrtle-green: #407376ff; 
$pear: #CED02Fff; 
$glaucous: #757CB4ff; 
$lemon-chiffon: #E0E2B8ff; 
$picton-blue: #19A1D9ff; 
/* SCSS HSL */ 
$myrtle-green: hsla(183, 30%, 36%, 1); 
$pear: hsla(61, 63%, 50%, 1); 
$glaucous: hsla(233, 30%, 58%, 1); 
$lemon-chiffon: hsla(63, 42%, 80%, 1); 
$picton-blue: hsla(197, 79%, 47%, 1); 
/* SCSS RGB */ 
$myrtle-green: rgba(64, 115, 118, 1); 
$pear: rgba(206, 208, 47, 1); 
$glaucous: rgba(117, 124, 180, 1); 
$lemon-chiffon: rgba(224, 226, 184, 1); 
$picton-blue: rgba(25, 161, 217, 1); /* SCSS Gradient */ 
$gradient-top: linear-gradient(0deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-right: linear-gradient(90deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-bottom: linear-gradient(180deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-left: linear-gradient(270deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-top-right: linear-gradient(45deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-bottom-right: linear-gradient(135deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, 
#19A1D9ff); 
$gradient-top-left: linear-gradient(225deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-bottom-left: linear-gradient(315deg, #407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff); 
$gradient-radial: radial-gradient(#407376ff, #CED02Fff, #757CB4ff, #E0E2B8ff, #19A1D9ff);`