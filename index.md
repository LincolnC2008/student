---
layout: default
title: Student Blog
---


## Lincoln Crowell's Page 
This is my blog for AP Computer Scinece Principles

![](<images/WIN_20230823_15_11_51_Pro.jpg>)

## About Me


- I have always lived in the US, however I have travelled and lived in many other countries longer than I have lived in the UK, hence the british flag in my picture.
- I have many hobbies but 1 hobby that is very important to me is fishing, I have gone fishing since I was 7 with my dad, and it is still something I like to do every summer.
- I have 2 sisters named Brooklyn and Zuzu, a mom named Cindy, and a dad named Jason. that is who the people in my picture are. We are all Chriastain which is where the cross comes from.
- Another hobby I have is gaming, I put that on there because it is also something I like to do with my sisters.
![](<images/IMG-2487.jpg>)


## I have a picture of me and my dad going fishing,  and on this day we caught a fish over 200lbs!

![](<images/IMG_1500.jpg>)

## This is a video I used to help me with coding

<iframe width="560" height="315" src="https://www.youtube.com/embed/wjbbl0TTMeo?si=hHdkr4Lk7XFZMw1u" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Problems I encountered while coding
I had encountered problems at the very start and a major problem being how I had not installed WSL Ubuuntu properly, WSL kept showing up with "root" so as a result I had to restart everything and reinstall the whole thing again. I am not certain, but I think the problem was when I made my username as I put the wrong one so I tried uninstalling, but I did not uninstall all the way so I looked up videos for help over the weekend until I eventually got it working. I had also encountered problems with inserting videos becasue when I was inserting the links, I did not realise they had to be embeded links so the videos would not work as it would say that the link is not found. As far as inserting pictures, I was struggling when copying the "link" to the picture as I did not realise when you drag and drop the photo into images you have to copy relative.

<body style="width=100px;border:1px solid red;">

Cookie Clicker
Credit: https://github.com/coderdojoindy/cookie-clicker/blob/master/index.html
<!DOCTYPE html>
<html>
<head>
<title>Cookie Clicker</title>
<!--
Code and graphics copyright Orteil, 2013
Feel free to alter this code to your liking, but please do not re-host it, do not profit from it and do not present it as your own.

-TODO :
	-milk toys
	-temple building
	-dungeons
	-gambling
	-better tooltips
	-better prestige
	-add canvas support
	-timer bars for golden cookie effects
	-set event listeners instead of onclick
	-more zebras
-->

<link rel="shortcut icon" href="img/favicon.ico" />
<link href="http://fonts.googleapis.com/css?family=Kavoon&subset=latin,latin-ext" rel="stylesheet" type="text/css">
<link href="style.css?v=1.5028" rel="stylesheet" type="text/css">

<script src="base64.js"></script>
<script src="ajax.js"></script>
<script src="dungeons.js?v=1.5026"></script>
<script src="main.js?v=1.5031"></script>


<script type="text/javascript">
  var _gaq = _gaq || [];
  _gaq.push(['_setAccount', 'UA-29324474-2']);
  _gaq.push(['_setDomainName', 'dashnet.org']);
  _gaq.push(['_trackPageview']);

  (function() {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
  })();
</script>

</head>
<body>

<div id="topBar">
	<div>
		<b>Cookie Clicker</b> &copy; <a href="http://orteil.dashnet.org" target="_blank">Orteil</a>, 2013 - hosted by <a href="http://dashnet.org" target="_blank">DashNet</a> | <a href="http://twitter.com/orteil42" target="_blank">twitter</a> | <a href="http://orteil42.tumblr.com" target="_blank">tumblr</a> | Help? Bugs? Ideas? Check out the <a href="http://forum.dashnet.org" target="_blank">forum</a>! | Chat with us on <a href="http://forum.dashnet.org/discussion/277/irc-chat-channel/p1" target="_blank">IRC</a> | Getting a black screen? Try pressing ctrl-F5!
		<div id="links" style="display:block;position:absolute;right:8px;top:4px;"></div>
	</div>
</div>

<div id="game">
	<div id="javascriptError">
		<div style="padding:64px 128px;">
			<div class="title">Oops, looks like the game isn't loading right!</div>
			<div>Please make sure your javascript is enabled, then refresh.<br>
			This could also be caused by a problem on our side, in which case - wait a moment, then refresh!</div>
		</div>
	</div>

	<div id="backgroundLayers">
		<div id="backgroundLayer1"></div>
		<div id="backgroundLayer2"></div>
	</div>
	
	<div id="goldenCookie" class="goldenCookie"></div>
	<div id="alert"></div>
	<div id="particles"></div>
	<div id="versionNumber" class="title"></div>
	
	<div id="sectionLeft" class="inset">
		<div id="cookieShower"></div>
		<div class="blackGradient"></div>
		<div class="blackFiller"></div>
		<div id="sectionLeftInfo"></div>
		<div id="cookies" class="title"></div>
		<div id="cookieAnchor">
			<div id="cookieShine"></div>
			<div id="cookieCursors"></div>
			<div id="bigCookie"></div>
			<div id="cookieNumbers"></div>
		</div>
		<div id="milk">
			<div id="milkLayer1" class="milkLayer"></div>
			<div id="milkLayer2" class="milkLayer"></div>
		</div>
	</div>

	<div class="separatorLeft"></div>
	<div class="separatorRight"></div>
		
	<div id="sectionMiddle" class="inset">
		<div id="comments" class="inset title">
			<div id="prefsButton" class="button">Menu</div>
			<div id="statsButton" class="button">Stats</div>
			<div id="logButton" class="button" style="font-size:80%;">Updates</div>
			<div id="commentsText"></div>
			<div class="separatorBottom"></div>
		</div>
		<div id="rows"></div>
		<div id="menu"></div>
	</div>

	<div id="sectionRight" class="inset">
		<div id="store">
			<div id="storeTitle" class="inset title">Store</div>
			<div id="upgrades">
			</div>
			<div id="products">
			</div>
		</div>
		
		<div id="support">
			<form action="https://www.paypal.com/cgi-bin/webscr" method="post" id="donate" style="margin:0px 16px;">
			<div id="supportComment">Help us make more games!</div>
			<input type="hidden" name="cmd" value="_s-xclick">
			<input type="hidden" name="hosted_button_id" value="BBN2WL3TC6QH4">
			<input type="image" src="https://www.paypalobjects.com/en_GB/i/btn/btn_donate_LG.gif" border="0" name="submit" alt="PayPal — The safer, easier way to pay online.">
			<img alt="" border="0" src="https://www.paypalobjects.com/nl_NL/i/scr/pixel.gif" width="1" height="1">
			</form>			
		</div>
	</div>
	
	<div id="tooltipAnchor"><div id="tooltip" onMouseOut="Game.tooltip.hide();"></div></div>

</div>

</body>
</html>