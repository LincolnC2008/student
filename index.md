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

// classes
// functions
// commands and global variables

// classes

class Clicker
{
	constructor()
	{
		this.level = 1
		this.price = 20;

		this.level_display = document.getElementById("clicker_level");
		this.price_display = document.getElementById("clicker_price");
		this.productivity_display = document.getElementById("clicker_productivity");

		this.renew_display();
	}

	click()
	{
		cookies += this.get_production_value();
		cookies_produced += this.get_production_value();
		renew_cookies();
	}

	get_production_value()
	{
		return Math.floor(1 + (0.05 * altogether_productivity * (this.level - 1)) + (this.level - 1));
	}

	improve()
	{
		if(cookies >= this.price)
		{
			cookies -= this.price;
			this.level += 1;
			this.price *= 2;
			this.renew_display();
		}
		else
		{
			alert("Not enough cookies!");
		}
	}

	renew_display()
	{
		this.level_display.innerHTML = this.level;
		this.price_display.innerHTML = this.price;
		this.productivity_display.innerHTML = this.get_production_value();
	}
}

class Building
{
	constructor(name, productivity, price)
	{
		this.name = name;
		this.level = 0;
		this.price = price;
		this.productivity = productivity;

		// variables for displaying
		// definition of areas
		this.area = document.createElement("span");
		this.area.id = name;

		this.level_display = document.createElement("span");
		this.level_display.id = this.name + "_level";

		this.productivity_display = document.createElement("span");
		this.productivity_display.id = this.name + "_productivity";

		this.price_display = document.createElement("span");
		this.price_display.id = this.name + "_price";

		this.button = document.createElement("button");
		this.button.innerHTML = "Improve";
	        this.button.onclick = this.improve.bind(this);

		// put together
		this.area.append(document.createTextNode(name + " Level: "));
		this.area.append(this.level_display);
		this.area.append(document.createElement("br"));

		this.area.append(document.createTextNode("Cookies per Second: "));
		this.area.append(this.productivity_display);
		this.area.append(document.createElement("br"));

		this.area.append(document.createTextNode("Improvement Price: "));
		this.area.append(this.price_display);
		this.area.append(document.createElement("br"));

		this.area.append(this.button);
		this.area.append(document.createElement("br"));
		this.area.append(document.createElement("br"));
        
        	setInterval(this.produce.bind(this), 1000);
	}
	
	get_price() 
	{
		return (this.price / 2) * (this.level * this.level + 1) + (this.price / 2) * (this.level + 1)
	}
	
	improve()
	{
        	if(cookies >= this.get_price())
        	{
        		cookies -= this.get_price();
        		this.level += 1;
        		altogether_productivity += this.productivity;
        		this.renew_display();
        		clicker.renew_display();
        	}
        	else
        	{
			alert("Not enough cookies!");
		}
	}

	renew_display()
	{
		this.level_display.innerHTML = this.level;
		this.productivity_display.innerHTML = this.get_production_value();
		this.price_display.innerHTML = this.get_price();
	}


	set_visible()
	{
		buildings.append(this.area);
		this.renew_display();
	}

	produce()
	{
		cookies += this.get_production_value();
		cookies_produced += this.get_production_value();
	}
	
	get_production_value()
	{
		return this.level * this.productivity;
	}
}

// functions

function renew_cookies()
{
	cookies_display.innerHTML = cookies;
	cookies_produced_display.innerHTML = cookies_produced;
    
	if(this.cookies_produced >= 200 && bakery_enabled == 0) 
	{
		bakery.set_visible();
		bakery_enabled = 1;
        
	}
	if(this.cookies_produced >= 2000 && factory_enabled == 0)
	{
		factory.set_visible(); 
		factory_enabled = 1;
	}
	if(this.cookies_produced >= 20000 && cookie_tesla_enabled == 0)
	{
		cookie_tesla.set_visible();
		cookie_tesla_enabled = 1;
	}

	if(this.cookies_produced >= 200000 && cookie_gigant_enabled == 0) 
	{
		cookie_gigant.set_visible(); 
		cookie_gigant_enabled = 1;
	}
}

// commands and (global) variables

var cookies = 0;
var cookies_produced = 0;
var altogether_productivity = 0; // counts productivity of buildings except clicker

var cookies_display = document.getElementById("cookies");
var cookies_produced_display = document.getElementById("cookies_produced");

var buildings = document.getElementById("buildings");

bakery_enabled = 0;
factory_enabled = 0;
cookie_tesla_enabled = 0;
cookie_gigant_enabled = 0;

clicker = new Clicker();
baker = new Building("Baker", 1, 20);
baker.set_visible();
bakery = new Building("Bakery", 10, 200);
factory = new Building("Factory", 100, 2000);
cookie_tesla = new Building("Cookie Tesla", 1000, 20000);
cookie_gigant = new Building("Cookie Gigant", 10000, 200000);

setInterval(renew_cookies, 500);

<html>
	<body>
		<b>Number of Cookies: <span id="cookies"></span></b><br>
		Cookies produced: <span id="cookies_produced"></span><br>
		<button onclick="clicker.click();">Make Cookie!</button><br><br>

		Clicker Level: <span id="clicker_level"></span><br>
		Production: <span id="clicker_productivity"></span><br>
		Improvement Price: <span id="clicker_price"></span><br>
		<button onclick="clicker.improve();">Improve</button><br><br>

		<hr><br>
		<span id="buildings"></span>

		<script src="main.js"></script>
	</body>
</html>