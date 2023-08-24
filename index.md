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
I had encountered problems at the very start and a major problem being how I had not installed WSL Ubuuntu properly, WSL kept showing up with "root" so as a result I had to restart everything and reinstall the whole thing again. I am not certain, but I think the problem was when I made my username as I put the wrong one so I tried uninstalling, but I did not uninstall all the way so I looked up videos for help over the weekend until I eventually got it working.

## A calculator I found
![credit] (<https://www.javatpoint.com/html-calculator>)  
<html>  
    <head>  
    <meta charset="utf-8">  
    <title>  
         Calculator using HTML Example  
    </title>  
    <link href="https://fonts.googleapis.com/css2?family=Cookie&display=swap" rel="stylesheet">  
    <!-- CSS property to create interactive  
        calculator interface -->  
    <style>  
    html {  
  height: 100vh;  
  display: flex;  
  align-items: center;  
  justify-content: center;  
  background-color: #2d3436;  
  background-image: linear-gradient(315deg, #2d3436 0%, #000000 74%);  
  font-family: 'Cookie', cursive;  
}  
.title {  
margin-bottom: 10px;  
padding: 5px 0;  
font-size: 40px;  
font-weight: bold;  
text-align: center;  
color: red;  
font-family: 'Cookie', cursive;  
}  
input[type=button] {  
  width: 60px;  
  height: 60px;  
  float: left;  
  padding: 0;  
  margin: 5px;  
  box-sizing: border-box;  
  background: #ecedef;  
  border: none;  
  font-size: 30px;  
  line-height: 30px;  
  border-radius: 50%;  
  font-weight: 700;  
  color: #5E5858;  
  cursor: pointer;    
}  
input[type=text] {  
  width: 270px;  
  height: 60px;  
  float: left;  
  padding: 0;  
  box-sizing: border-box;  
  border: none;  
  background: none;  
  color: red;  
  text-align: right;  
  font-weight: 700;  
  font-size: 60px;  
  line-height: 60px;  
  margin: 0 25px;  
  }  
.calculator {  
  background-color: #c0c0c0;  
  box-shadow: 0px 0px 0px 10px #666;  
  border: 5px solid black;  
  border-radius: 10px;  
}  
#display {  
  height: 40px;  
  text-align: right;  
  background-color: black;  
  border: 3px solid white;  
  font-size: 18px;  
  left: 2px;  
  top: 2px;  
  color: red;  
}  
.btnTop {  
  color: white;  
  background-color: #6f6f6f;  
  font-size: 14px;  
  margin: auto;  
  width: 50px;  
  height: 25px;  
}     
    </style>  
</head>  
<body>  
    <div class = "title"  align="center">  
        Example of Calculator using HTML  
    </div>  
    <form name="Calculator" class = "calculator" >  
<table border="2" align="center" cellpadding="15" cellspacing="12" bgcolor="#c0c0c0">  
<tr>  
<td>  
<input type="text" name="Input" Size="35" id="display">  
<br>  
</td>  
</tr>  
<tr>  
<td>  
<input type="button" name = "one" style="font-size:30px" value=" 1 " OnClick="Calculator.Input.value += '1'">  
<input type="button" name = "two" style = "font-size:30px" value=" 2 " OnCLick="Calculator.Input.value += '2'">  
<input type="button" name = "three" style="font-size:30px" value=" 3 " OnClick="Calculator.Input.value += '3'">  
<input type="button" name="add" class ="btnTop" style="font-size:30px" value=" + " OnClick="Calculator.Input.value += ' + '">  
<br>  
<input type="button" name = "four" style="font-size:30px" value=" 4 " OnClick="Calculator.Input.value += '4'">  
<input type="button" name = "five" style="font-size:30px" value=" 5 " OnCLick="Calculator.Input.value += '5'">  
<input type="button" name = "six" style="font-size:30px" value=" 6 " OnClick="Calculator.Input.value += '6'">  
<input type="button" name = "minus" style="font-size:30px" value=" - " OnClick="Calculator.Input.value += ' - '">  
<br>  
<input type="button" name = "seven" style="font-size:30px" value=" 7 " OnClick="Calculator.Input.value += '7'">  
<input type="button" name = "eight" style="font-size:30px" value=" 8 " OnCLick="Calculator.Input.value += '8'">  
<input type="button" name = "nine" style="font-size:30px" value=" 9 " OnClick="Calculator.Input.value += '9'">  
<input type="button" name = "mul" style="font-size:30px" value=" * "   
OnClick="Calculator.Input.value += ' * '">  
<br>  
<input type="button" name = "clear" style="font-size:30px" value=" c " OnClick="Calculator.Input.value = ''">  
<input type="button" name="zero" style="font-size:30px" value=" 0 " OnClick="Calculator.Input.value += '0'">  
<input type="button" name="DoIt" style="font-size:30px" value=" = " OnClick="Calculator.Input.value = eval(Calculator.Input.value)">  
<input type="button" name="div" style="font-size:30px" value=" / " OnClick="Calculator.Input.value += ' / '">  
<br>  
</td>  
  
</tr>  
</table>  
</form>  
</body>  
</html>     