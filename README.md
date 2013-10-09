HELP-WEBSITE--
==============

Hi. everybody

I would like to give some little support, please to the development of my website. This email is the same of your email given on linkedin.

It´s only two simple questions. It´s no longer than 5 or 10 minutes to solve it. The questions are the following:

On the files website- IE and the website- Google chrone, my doubt is: 

1) The width and the height of the website don´t follow the width and the height of all the screen of the computer. That means the width and the height in both cases don´t correspond to the limits of the screen of the computer. Send me the code to correct this situation. 

2) The chat, must be on the right corner bonded (glued) to the footer of the website as mentioned on the word file (chat). Send me the code to correct this situation. 

I could count with your support because this website that iam creating is to porpose to creat a personal marketing to find a job or a professional trainning. I expect your answer as soon as posible.

PS.: The files (compressed by ZIP) of my website are on your email given on linkedin. And my informatic tools are: DREAMWEAVER and WAMPSERVER to visualize the website on GOOGLE CHROME and INTERNET EXPLORER. 

Best regards 

Have a nice weekend 

José Moreira


The code of my website is on below:

layout.html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>Untitled Document</title>
<link href="site.css" rel="stylesheet" type="text/css" />
<style type="text/css">
.calendarTable {
    background-color:#eee;
    color:#333;
    border: 1px solid #bbb;
	width: 100px;
	margin-left:auto;
	margin-right:auto;
}
.calendarTable td {
    text-align: center;
    padding: 2px 1px 2px 1px;
}
.calendarTable td.monthHead {
    font-weight: bold;
    border: 1px solid #bbb;
    background-color:#ddd;
}
.calendarTable td.weekDay {
    font-weight: bold;
}
.calendarTable td.monthDay {
    border: 1px solid #ddd;
}
.calendarTable td.currentDay {
    font-weight: bold;
    color:#ad5;
    border: 1px solid #aaa;
}
</style>
<script type="text/javascript" language="javascript">
/** Function to display a Calendar based on javascript. **/
function calendar() {
  // Get the current date parameters.
  var date = new Date();
  var day = date.getDate();
  var month = date.getMonth();
  var year = date.getFullYear();
  
  var months = new Array('January','February','March','April','May','June','July','August','September','October','November','December');
  var monthDays = new Array(31,28,31,30,31,30,31,31,30,31,30,31);
  var weekDay = new Array('Mo','Tu','We','Th','Fr','Sa','Su');
  var days_in_this_month = monthDays[month];

  // Create the basic Calendar structure.
  var calendar_html = '<table class="calendarTable">';
  calendar_html += '<tr><td class="monthHead" colspan="7">' + months[month] + ' ' + year + '</td></tr>';
  calendar_html += '<tr>';
  var first_week_day = new Date(year, month, 1).getDay();
  for(week_day= 0; week_day < 7; week_day++) {
    calendar_html += '<td class="weekDay">' + weekDay[week_day] + '</td>';
  }
  calendar_html += '</tr><tr>';

  // Fill the first week of the month with the appropriate number of blanks.
  for(week_day = 0; week_day < first_week_day; week_day++) {
    calendar_html += '<td> </td>';
  }
  week_day = first_week_day;
  for(day_counter = 1; day_counter <= days_in_this_month; day_counter++) {
    week_day %= 7;
    if(week_day == 0)
      calendar_html += '</tr><tr>';
    // Do something different for the current day.
    if(day == day_counter) {
      calendar_html += '<td class="currentDay">' + day_counter + '</td>';
    } else {
      calendar_html += '<td class="monthDay"> ' + day_counter + ' </td>';
 }
    week_day++;
  }
  calendar_html += '</tr>';
  calendar_html += '</table>';
  // Display the calendar.
  document.write(calendar_html);
}
</script>

<!-- This part can go in the head of the html file -->

<script language="JavaScript" type="text/javascript">
<!-- Copyright 2003, Sandeep Gangadharan -->
<!-- For more free scripts go to http://sivamdesign.com/scripts/ -->
<!--

function sivamtime() {
  now=new Date();
  hour=now.getHours();
  min=now.getMinutes();
  sec=now.getSeconds();

if (min<=9) { min="0"+min; }
if (sec<=9) { sec="0"+sec; }
if (hour>12) { hour=hour-12; add="pm"; }
else { hour=hour; add="am"; }
if (hour==12) { add="pm"; }

document.timeForm.field.value = ((hour<=9) ? "0"+hour : hour) + ":" + min + ":" + sec + " " + add;

setTimeout("sivamtime()", 1000);
}
window.onload = sivamtime;
</script>


</head>
<body>
<div id="layout"> <!-- see the css code from site.css -->
	<div><!--Let this div so it is. This conteiner holds the header divs of your site.-->
		<div id="topo"><img src="images/jose.jpg" width="960" height="100" alt="Jose Moreira" /></div>
		
		<div id="bandeiras">
			<!-- We give for all img tag the class "class="top_right_menu" and set up the width, height, padding and border in stylesheet (site.css)-->
			<div class="top_right_menu">	
				<img src="images/mapadosite.jpg" class="top_right_menu" alt="mapa do site" />
				<img src="images/home.jpg" class="top_right_menu" alt="home" />
				<img src="images/rss.jpg" class="top_right_menu" alt="rss" />
				<img src="images/portugues.jpg" class="top_right_menu" alt="português" />
				<img src="images/ingles.jpg" class="top_right_menu" alt="inglês" />
				<a href="http://www.facebook.com">
					<img src="images/facebook.jpg" class="top_right_menu" alt="facebook" />
				</a>
				<a href="http://www.linkedin.com">
					<img src="images/linkedin.jpg" class="top_right_menu" alt="linkedin" />
				</a>
				<a href="https://twitter.com">
					<img src="images/twiter.jpg" class="top_right_menu" alt="twitter" />
				</a>
			</div>	
		</div>
	</div>
	
	<div class="page_content"><!-- Here are the divs with the page content. For its settings see the site.css file please.-->
		<!-- First we put a div_left with your menu and "dashboard" data -->
		<div class="div_left"><!--Within this div is established center alignment of the menu, calendar, clock, weather, aso (see the code from site.css )-->
			<div id="menu_navegacao"> 
				<p>
					<a href="#">Introdução</a> <a href="#">Clientes</a> <a href="#">Novidades</a> <a href="#">Contato </a>
				</p>
			</div>

			<!--calendar -->
			<!--Do not use anymore <center> tag. It is deprecated tag. -->
			<div class="data_info"> <!-- For calendar and clock-->
				<script type="text/javascript">calendar();</script></center>

				<!--clock -->

				<!--Do not use anymore <center> tag. It is deprecated tag. 
				To center a conteiner please use div or span with the property margin-left and margin-right with the value auto -->
				<!-- Why did you use the form only for a text input tag? You can use the text input box without the form.-->
				<form name="timeForm">
					<input type=text" name="field" value="" size="10">
				</form>
			</div>		
				
			<!--weather -->
			<div class="weather">
					<div id="cont_44195f23474f208a222d258bb1143f4d" >
						<span id="h_44195f23474f208a222d258bb1143f4d">
							<a id="a_44195f23474f208a222d258bb1143f4d" href="http://www.tempo.pt/" target="_blank" style="color:#808080;font-family:Times New Roman;font-size:14px;">Clima</a> Viana do Castelo
						</span>
						<script type="text/javascript" src="http://www.tempo.pt/wid_loader/44195f23474f208a222d258bb1143f4d"></script>
					</div>
			</div>	

			<div class="dashboard">
				<!--visits counter -->

				<!-- Do not use any more <center> tag because is deprecated -->
				<table border="1" cellpadding="0" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="13%" id="AutoNumber1" height="27"> 
				  <tr> 
					<td width="100%" height="27">
						<script language="javascript" src="http://www.countads.com/count.php?id=791&cmd=cookie"></script> 
						<p align="center"> 
							<img src="http://www.countads.com/count.php?id=791&cmd=img_only" border="0" width="172" height="21" ><br /><!-- According to XHTML rules the brake line tag is written so: <br /> --> 
							<span style="font-family: arial, verdana, sans-serif; font-size: 8pt"> 
								<a href="http://www.ocio-full.blogspot.com"></a>
							</span>
					</td> 
				  </tr> 
				</table>

				<!--radio online -->

				<div id="container">
					<a href="http://www.macromedia.com/go/getflashplayer">Get the Flash Player</a> to see this player.
					<a href="http://www.shoutcheap.com/shoutcast/">shoutcheap shoutcast server hosting</a>
					<a href="http://www.shoutcheap.com/icecast/">shoutcheap icecast server hosting</a>
				</div>
			</div>	
			
			<script type="text/javascript" src="http://www.shoutcheap.com/flashplayer/swfobject.js"></script>
			<script type="text/javascript">
				var s1 = new SWFObject("http://www.shoutcheap.com/flashplayer/player.swf",
				"ply","174","30","9","#FFFFFF");
				s1.addParam("allowfullscreen","true");
				s1.addParam("allowscriptaccess","always");
				s1.addParam("flashvars",
				"file=http://ipaddress:port/;stream.nsv&type=mp3&volume=50&autostart=true");
				s1.write("container");
			</script>
		
		</div>
		
	</div>
	
	<div id="conteudo">
		<h3>Apresentation</h3>
	 
		<p>This site was build with the intention of it being a sharing with other people, 
		being my personnel marketing and I also consider being one demonstration of my learning process of new knowledges 
		in different programming languages as HTMl and Javascript, althought my basic formation it is a degree in Sociology. 
		However I would be very grateful with your suggestions and opinions, because there are always aspects to change if 
		we want to make progress to become better and to improve our skills. Thus your feedback is important.   
		</p>

		<!--   chat    -->
		<p>
			<a id="ewclink" href="http://www.everywherechat.com/"></a> 
 			<script src="http://www.everywherechat.com/e.php?defaultRoom=Lobby&roomList=true&fontSize=10&width=290&height=170&theme=night">
			</script>
		</p>
	</div>
	
	
</div>

<!--footer -->
<div id="rodape">
	<p></p>
</div>
</body>
</html>

css.html
/* CSS Document */
#topo img {
	height: auto;
	width: 100%;
}
#bandeiras {
	height:22px;
	background-color:#09F;
	padding:0px;
	text-align:right;
}

div.top_right_menu
{
float:right;
width:auto;
height:21px;
padding:0px;
background-color:#FFFFFF;
}

div.top_right_menu a:link, a:visited, a:hover, a:active
{
width:36px;
height:21px;
text-decoration:none;
}

img.top_right_menu
{
float:left;
width:30px;
height:15px;
padding:2px;
border:1px solid #09F;
}


.page_content /*This conteiner contains the divs with the page content*/
{
display:block;
text-align;center;
}

.div_left/*This conteiner contains the divs with the menu, calendar, clock, weather aso*/
{
float:left;
width:auto;
height:auto;
text-align:center;
}


#menu_navegacao/*setting code for div with the menu*/
{
display:block;
width:174px;/*this is equal with the width + 2*margin + 2*padding from a #menu_navegacao (see bellow) */
height:auto;
margin-left:auto;
margin-right:auto;
}

/*Please use code also for a:visited*/
#menu_navegacao a:link {
	display: block;
	width: 150px;
	height: 20px;
	margin: 2px;
	padding: 10px;
	font-family: Verdana, Geneva, sans-serif;
	font-size: 12px;
	font-style: normal;
	font-weight: bold;
	text-transform: capitalize;
	color: #FFF;
	text-decoration: none;
	background-color: #09C;
	border: thin solid #999;
}

/*please use code also for a:active*/
#menu_navegacao a:hover {
	background-color: #A6E9FF;
	color: #000000;
/*	
 the bellow code does not be mentioned because the effect is set through code from a:link
	font-family: Verdana, Geneva, sans-serif;
	font-size: 12px;
	font-style: normal;
	font-weight: bold;
	text-transform: capitalize;
	text-decoration: none;
	display: block;
	margin: 2px;
	padding: 10px;
	height: 20px;
	width: 150px;
	border: thin solid #999;
*/	
}

.data_info, .dashboard/*setting code for div with calendar and clock*/
{
display:block;
width:174px;/*This is the width of the div for menu*/
height:auto;
text-align:center;
margin-left:auto;
margin-right:auto;
}

.weather/*setting code for div with calendar, clock, weather aso*/
{
display:block;
width:70px;/*This is the width of the div for menu*/
height:auto;
margin-left:auto;
margin-top:5px;
margin-right:auto;
margin-bottom:5px;
text-align:center;
}

#conteudo {
	background-color: #E6E6E6;
	clear: right;
	float: right;
	height: 800px;
	width: 750px;
	text-align: left;
}
#rodape {
	font-family: Verdana, Geneva, sans-serif;
	font-size: 12px;
	font-weight: normal;
	color: #FFF;
	background-color: #000;
	text-align: center;
	display: block;
	width: 960px;
	height: 20px;
	margin-left:auto;/*Modified by Radu*/
	margin-right:auto;/*Modified by Radu*/
	clear: both;
}
#layout {
	
	width: 960px;/*Why did you use 960px width resolution? Now the minimum resolution is 1024x768. See http://www.w3schools.com/browsers/browsers_display.asp*/
	height:auto;/*Modified by Radu*/
	margin-left:auto;/*Modified by Radu*/
	margin-right:auto;/*Modified by Radu*/
/* height: 650px; this code does not have to appear*/
/* overflow: auto; this code does not have to appear*/
/* z-index: auto; this code does not have to appear*/
}
#conteudo p #ewclink {
	text-align: right;
}
#phead {
	font-family: "Times New Roman", Times, serif;
	font-size: 36px;
	font-style: normal;
	text-align: center;
}
#conteudo h3 {
	text-align: center;
	font-weight: bold;
	font-style: italic;
	font-size: 36px;
	font-family: "Times New Roman", Times, serif;
}
#conteudo p {
	text-align: justify;
	position: static;
	right: 30px;
	letter-spacing: 3px;
	font-weight: normal;
	clear: none;
	float: none;
	margin-left: 25px;
	margin-right: 25px;
	color: #009;
	font-size: 18px;
}






