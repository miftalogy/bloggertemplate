/* 
  Name: Gothica Blogger Template
  Author: Virtuti-D
  Author URI: http://www.virtuti.info/ 
  Version: 1.0.1
  Date: April, 2013
  License: commercal, not for redistrubution, reselling.
*/   
/* ------------------------------------------------------------------------------------
--  RESET
------------------------------------------------------------------------------------ */
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, img, ins, kbd, q, s, samp,
small, strike, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
table {
    border-collapse: collapse;
    border-spacing: 0;
}
/* ------------------------------------------------------------------------------------
--  GENERAL 
------------------------------------------------------------------------------------ */
html, body{ 
    width:100%;
	margin: 0; 
	padding: 0;
	line-height:normal;
	font-size:100%;
    font-family: 'Enriqueta', Georgia, serif;
	color:#808080;
    background: #000 url(images/bg.jpg) no-repeat top left fixed; 
    background-size: cover;
}

@media screen and (max-width: 1440px) {
    html, body{
	font-size:95%;
  }
}
/* 1.25 dpr */
@media 
(-webkit-min-device-pixel-ratio: 1.25), 
(min-resolution: 120dpi){ 
html, body{ 
	background-size:contain;
}
}

/* 1.3 dpr */
@media 
(-webkit-min-device-pixel-ratio: 1.3), 
(min-resolution: 124.8dpi){ 
html, body{ 
	background-size:contain;
}
}

/* 1.5 dpr */
@media 
(-webkit-min-device-pixel-ratio: 1.5), 
(min-resolution: 144dpi){ 
html, body{ 
	background-size:contain;
}
}
::selection{
	color:#fafafa;
	background:#000;
}
::-moz-selection{
	background:#eee;
	color:#000;
}
img{
    display:block;
	max-width:100%;
	height:auto;
}
a{
	color:#214b70;	
	text-decoration:none;
	-moz-transition: 500ms ease-in;
    -o-transition: 500ms ease-in;
    -webkit-transition: 500ms ease-in;
    -ms-transition: 500ms ease-in;
    transition: 500ms ease-in; 	
}
a:hover, 
a:focus{
	color:#356793;
}
h1, h2, h3, h4, h5, h6{
   font-weight:normal;
}
/* ------------------------------------------------------------------------------------
--  EVERYTHING BLUE 
------------------------------------------------------------------------------------ */
.circle,
.line,
.label,
.date-header span,
.blog-pager-menu a, 
a.totop, 
a.trigger,
.post-body:after{
	background:#356793;
	background:-webkit-linear-gradient(top, #356793 0%, #214b70 100%);
    background: -moz-linear-gradient(top, #356793 0%, #214b70 100%);
    background: -o-linear-gradient(top, #356793 0%, #214b70 100%);
    background: -ms-linear-gradient(top, #356793 0%, #214b70 100%);
    background: -khtml-linear-gradient(top, #356793 0%, #214b70 100%);
}
.blue{
    color:#356793;
}
.colorchange{
    -webkit-animation: 9s colorchange infinite alternate;
    -moz-animation: 9s colorchange infinite alternate;
    -o-animation: 9s colorchange infinite alternate;
     animation: 9s colorchange infinite alternate;	
}
@-webkit-keyframes colorchange{
  from { background: #1375c6}
  to { background: #2b5880}
}
@-moz-keyframes colorchange{
  from { background: #1375c6}
  to { background: #2b5880}
}
@-o-keyframes colorchange{
  from { background: #1375c6}
  to { background: #2b5880}
}
@keyframes colorchange{
  from { background: #1375c6}
  to { background: #2b5880}
}
@media screen and (max-width: 799px) {
.colorchange{
    -webkit-animation: 0s colorchange infinite alternate;
    -moz-animation: 0s colorchange infinite alternate;
    -o-animation: 0s colorchange infinite alternate;
     animation: 0s colorchange infinite alternate;	
}
}
/* ------------------------------------------------------------------------------------
--  MAIN WRPPER STRUCTURE
------------------------------------------------------------------------------------ */
#main-wrapper{
	position:absolute;
	width:100%;
	top:0;
	left:0;
}
@media screen and (max-width: 799px) {
#main-wrapper{
	float:left;
	width:100%;
	clear:both;
	position:relative;
}
}
#nav-wrap{
	width:12%;
	top:0;
	left:0;
	position:fixed;
	height:100%;
	min-height:100%;
}
@media screen and (max-width: 1440px) {
#nav-wrap{
	width:10%;
  }
}
@media screen and (max-width: 1024px) {
#nav-wrap{
	width:12%;
  }
}
@media screen and (max-width: 799px) {
#nav-wrap{
	float:left;
	width:100%;
	top:0;
	left:0;
	position:relative;
}
}
#main-box-wrap{
	float:left;
	position:relative;
	width:88%;
	left:12%;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	border-right:50px solid transparent;
}
@media screen and (max-width: 1440px) {
#main-box-wrap{
	width:90%;
	left:10%;
  }
}
@media screen and (max-width: 1024px) {
#main-box-wrap{
	width:88%;
	left:12%;
  }
}
@media screen and (max-width: 799px) {
#main-box-wrap{
	width:100%;
	left:0;
	border-right:none;
  }
}
/* ------------------------------------------------------------------------------------
--  CONTENT WRAPPER
------------------------------------------------------------------------------------ */
#content-wrapper{
	float:left;
	width:100%;
}
/* ------------------------------------------------------------------------------------
--  CONTENT BOX
------------------------------------------------------------------------------------ */
#main-box{
	float:left;
	width:60%;
	background:rgba(0,0,0,0.7);
}
@media screen and (max-width: 1600px) {
#main-box{
	width:66%;
  }
}
@media screen and (max-width: 1024px) {
#main-box{
	width:100%;
  }
}
#sidebar-box{
	float:left;
	width:26%;
}
@media screen and (max-width: 1600px) {
#sidebar-box{
	width:32%;
  }
}
@media screen and (max-width: 1024px) {
#sidebar-box{
	width:100%;
  }
}
/* ------------------------------------------------------------------------------------
--  SCROLL TO TOP BUTTON
------------------------------------------------------------------------------------ */
#totop{
	width:12%;
	position:fixed;
	bottom:40px;
	z-index:5;
}
@media screen and (max-width: 1440px) {
#totop{
	width:10%;
  }
}
@media screen and (max-width: 1024px) {
#totop{
	width:12%;
  }
}
@media screen and (max-width: 799px) {
#totop{
	display:none;
  }
}
#totop span{
	width:100%;
	float:left;	
}
#totop a{
	display:table;
	margin:0 auto;
	box-shadow:inset 0 0 4px rgba(0,0,0,0.2);
	border:1px solid rgba(255,255,255,0.05);	
	height:32px;
	width:32px;
}
#totop a img{
	height:32px;
	width:32px;	
}
/* ------------------------------------------------------------------------------------
--  NAVIGATION
------------------------------------------------------------------------------------ */
nav{
	float:left;
	width:100%;
	margin:240px 0 0 0;
}
@media screen and (max-width: 1440px) {
nav{
	margin:160px 0 0 0;
  }
}
@media screen and (max-width: 1024px) and (max-height:600px) {
nav{
	margin:40px 0 0 0;
  }
}
@media screen and (max-width: 799px) {
nav{
	float:left;
	width:90%;
	background:#356793;
}
}
/*-----------blogger class starts-----------*/
.PageList{
	float:left;
	width:100%;	
}
.PageList ul{
	display:table;
	margin:0 auto;
	list-style:none;
	width:100px;
}
@media screen and (max-width: 1366px) {
.PageList ul{
	width:80px;
  }
}
@media screen and (max-width: 1024px) {
.PageList ul{
	width:70px;
  }
}
@media screen and (max-width: 799px) {
.PageList ul{
	width:100%;
  }
}
.PageList ul li{
	float:left;
	width:100%;
	display:block;
}
.PageList h2{
	display:none;
}
/*-----------blogger class ends-----------*/
.circle{
	float:left;
	width:100px;
	height:100px;
	border-radius:50%;
	text-align:center;
	line-height:80px;
	box-shadow:0 4px 20px rgba(0,0,0,0.9);
	margin-bottom:20px;
}
@media screen and (max-width: 1366px) {
.circle{
	width:80px;
	height:80px;
	line-height:60px;
  }
}
@media screen and (max-width: 799px) {
.circle{
	float:left;
	width:100%;
	height:auto;
	border-radius:0;
	text-align:center;
	line-height:normal;
	box-shadow:none;
	margin:0;
	text-align:left;
}
}
.circle:last-child{
	margin-bottom:0;
}
.circle a{
	float:left;
	width:80px;
	height:80px;
	border-radius:50%;	
	margin:10px;
	background:#356793;
	font-family:'Oswald', sans-serif;
	text-transform:uppercase;
	font-size:0.8em;
	color:#f0f0f0;
	letter-spacing:0.1em;
}
@media screen and (max-width: 1366px) {
.circle a{
	width:60px;
	height:60px;
	font-size:0.75em;
  }
}
@media screen and (max-width: 799px) {
.circle a{
	float:left;
	display:block;
	width:100%;
	height:auto;
	border-radius:0;
	margin:0;
	padding:16px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	border-top:1px solid rgba(255,255,255,0.05);
    border-bottom:1px solid #2b5880;
    font-size:0.9em;

  }
}
.circle a:hover,
.circle a:focus{
    color:#fff;
}
/* ------------------------------------------------------------------------------------
--  MOBILE NAVIAGTION
------------------------------------------------------------------------------------ */
#ntrigger{
	text-align:center;
	padding:10px;
	width:20px;
	height:20px;
	margin:0 0 60px 0;
	display:none;
}
@media screen and (max-width: 799px) {
#ntrigger{
     display: block;
  }
}
#ntrigger .plus p{
	width:20px;
	background:#f0f0f0;
	height:4px;
	margin:0 0 4px 0;
}
#ntrigger .plus p:last-of-type{
	margin:0;
}
#ntrigger .close{
	font-size:18px;
}
.navplace{
	float:left;
	width:100%;
    height:auto;	
}
@media screen and (max-width: 799px) {
.navplace{
     display:none;
  }
}
/* ------------------------------------------------------------------------------------
--  OPENING PANEL
------------------------------------------------------------------------------------ */
#panel-wrap{
    float:left;
    /*width:420px;/*--------because of adSense 300px wide-----*/
    width:100%;
    position:relative;
}
a.trigger{
	display:block;
	text-align:center;
	box-shadow:inset 0 0 4px rgba(0,0,0,0.2);
	border:1px solid rgba(255,255,255,0.07);	
	color:#f0f0f0;	
}
#strigger-place{
	position:fixed;
	width:50px;
	height:100%;
	min-height:100%;
	right:0;
	top:45%;
}
#strigger{
	display:block;	
    width:50px;
	height:50px;
	line-height:50px;
	font-size:26px;
}
@media screen and (max-width: 1024px) {
#strigger{
	display:none;
	width:0;
  }
}
a.trigger .close{
	display:none;	
}
a.active.trigger .close{
    display:inline;
}
a.active.trigger .plus{
	display:none;
}
.panel{
	float:left;
	width:100%;
    display: none;
	background:#ddd;
    height: auto;	
	padding:30px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	line-height:1.5em;
}
@media screen and (max-width: 1023px) {
.panel{
    display: block;
  }
}
/* ------------------------------------------------------------------------------------
--  SIDE TITLE
------------------------------------------------------------------------------------ */
#title-wrap{
	position:fixed;
	bottom:30px;
	right:40px;
	-webkit-animation-delay:2s;
	 animation-delay:2s;
}

#title-wrap p{
	-moz-transition: 500ms ease-in;
    -o-transition: 500ms ease-in;
    -webkit-transition: 500ms ease-in;
    -ms-transition: 500ms ease-in;
    transition: 500ms ease-in; 
	font-size:8em;
    font-family: 'UnifrakturMaguntia', cursive;
	color:#d6a754;
	line-height:normal;
    -webkit-text-stroke: 1px rgba(234,222,185,0.5); /*#f3deb9*/
    -moz-text-stroke: 1px rgba(234,222,185,0.5); /*#f3deb9*/
    -o-text-stroke: 1px rgba(234,222,185,0.5); /*#f3deb9*/
    -ms-text-stroke: 1px rgba(234,222,185,0.5); /*#f3deb9*/
    text-shadow:
               0 1px 0 #bd9042, 
               0 2px 0 #c18b2d,
               0 4px 0 #7f5813,
               0 5px 0 #d28806,
               0 6px 0 #573a08,
               0 8px 1px rgba(0,0,0,.1),
               0 0 5px rgba(0,0,0,.1),
               0 1px 3px rgba(0,0,0,.3),
               0 3px 5px rgba(0,0,0,.2),
               0 5px 10px rgba(0,0,0,.25),
               0 10px 10px rgba(0,0,0,.2),
               0 20px 20px rgba(0,0,0,.15);
}
@media screen and (max-width: 1366px) {
#title-wrap p{
	font-size:7em;
  }
}
@media screen and (max-width: 1280px) {
#title-wrap p{
	font-size:6.8em;
  }
}
@media screen and (max-width: 1279px) {
#title-wrap p{
	display:none;
  }
}
/* ------------------------------------------------------------------------------------
--  HEADER 
------------------------------------------------------------------------------------ */
header{
	float:left;
	width:100%;
	background-repeat:repeat;
	border-bottom:8px solid rgba(255,255,255,0.09);
	text-align:center;
}
/*-----------blogger class starts-----------*/
.Header{
	float:left;
	width:100%;
	margin:0;
	padding:0;
	z-index:5;
	background:#141414 url(images/pattern.png);
}
#header-inner{
	display:table;
	margin:50px auto;
}
.titlewrapper{
	float:left;
	width:100%;
}
header h1.title{
	font-size:1.6em;	
	letter-spacing:0.1em;
	color:#1375c6;	
	font-family: 'Monda', sans-serif;
	text-transform:uppercase;
	line-height:1.2em;
}
header h1.title a{
	color:#1375c6;
	display:inline-block;	
}
/*-----------blogger class ends-----------*/
.line{
	float:left;
	width:100%;
	height:5px;
}
/*-----------blogger class starts-----------*/
.descriptionwrapper{
	float:left;
	width:100%;
}
.descriptionwrapper p.description{
	padding:0;
	margin:20px 0 0 0;
	font-family:'Monda', sans-serif;
	text-transform:uppercase;
	font-size:0.9em;
	color:#aaa;
	letter-spacing:0.2em;
}
/*-----------blogger class ends-----------*/
/* ------------------------------------------------------------------------------------
--  SUB NAVIGATION 
------------------------------------------------------------------------------------ */
/*-----------blogger class starts-----------*/
#subnav{
    float:left;
    width:100%;	
}
#main0{
    float:left;
    width:100%;	
}
#main0 .Label{
    float:left;
    width:100%;
    margin:0;
    padding:0;
}
#main0 .Label ul{
	list-style:none;
	float:left;
	width:100%;
	padding:0;
	text-align:center;
	margin:0 0 40px 0;
	background:#181511 url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQIW2NgYGB4z4AAFUhsFAG4IsICMIBiLgBmEQcEyASpFQAAAABJRU5ErkJggg==);
	border-bottom:1px solid rgba(255,255,255,0.07);
}
#main0 .Label li{
	float:left;
	padding:16px 0;
	width:20%;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	border-right:1px solid rgba(255,255,255,0.07);
}
@media screen and (max-width: 639px) {
#main0 .Label li{
	border-right:none;	
  }
}
#main0 .Label li:last-child{
    border-right:none;
}
#main0 .Label a{
	color:#1c6aab;	
	font-family:'Oswald', sans-serif;
	text-transform:uppercase;
	font-size:0.9em;	
	letter-spacing:0.1em;
}
@media screen and (max-width: 639px) {
#main0 .Label a{
	display:none;	
  }
}
#main0 .Label a:hover
#main0 .Label a:focus{
	color:#2486d7;
}
#main0 .Label span{
	font-family:'Oswald', sans-serif;
	text-transform:uppercase;
	font-size:0.9em;	
	letter-spacing:0.1em;
	color:#3BA2F7;
}
#main0 .Label h2{
	display:none;
}
/*-----------blogger class ends-----------*/
/* ------------------------------------------------------------------------------------
--  POST BLOCK
------------------------------------------------------------------------------------ */
/*-----------blogger class starts-----------*/
.Blog{
	float:left;
	width:100%;
	font-size:120%;
}
@media screen and (max-width: 1600px) {
.Blog{
	font-size:115%;
  }
}
.date-outer{
	float:left;
	width:100%;
	margin:0 0 30px 0;
}
/* ------------------------------------------------------------------------------------
--  POST 
------------------------------------------------------------------------------------ */
.post{
	float:left;
	width:100%;
	background:#070605;
}
.post a{
	color:#3BA2F7;
}
.post a:hover
.post a:focus{
	color:#2486d7;
}
/* ------------------------------------------------------------------------------------
--  POST BLOCK: DATE
------------------------------------------------------------------------------------ */
h2.date-header{
	display:block;
	width:96%;
	margin:0 4% 0 0;
}
h2.date-header span{
	float:right;
	padding:10px 20px;
	color:#b1b1b1;
	font-size:0.9em;
}
/* ------------------------------------------------------------------------------------
--  POST BLOCK: POST TITLE
------------------------------------------------------------------------------------ */
.post h3.post-title{
	float:left;
	width:92%;
	font-family:"Monda", sans-serif;
	text-transform:uppercase;
	background:#070605;
	padding:20px 4%;
	letter-spacing:0.1em;
	color:#aaa;
}
.post h3.post-title a{
	color:#aaa;	
}
.post h3.post-title a:hover,
.post h3.post-title a:focus{
	color:#356793;
}
/*-----------blogger class ends-----------*/
/* ------------------------------------------------------------------------------------
--  POST BODY
------------------------------------------------------------------------------------ */
/*-----------blogger class starts-----------*/
.post-body{
	float:left;
	width:96%;
	background:#f0f0f0;
	border-top:8px solid #356793;
	position:relative;
	padding:30px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	line-height:1.5em;
	font-size:105%;
}
@media screen and (max-width: 799px) {
.post-body{
	width:100%;
}
}
/*-----------blogger class ends-----------*/
.post-body:after{
	content:'✑';
	color:#f0f0f0;
	position:absolute;
	top:38px;
	right:-4%;
	width:4%;
	height:40px;
	line-height:40px;
	text-align:center;
}
@media screen and (max-width: 799px) {
.post-body:after{
	display:none;
}
}
/* ------------------------------------------------------------------------------------
--  POST BODY STYLES
------------------------------------------------------------------------------------ */
.post-body b, 
.post-body strong{
	font-weight:700;
}
.post-body sub, 
.post-body sup{
    font-size: 75%;
	line-height: 0;
	position: relative;
	vertical-align: baseline
}
.post-body sup{
	top: -0.5em
}
.post-body sub {
	bottom: -0.25em
}
.post-body a{
	color:#7baad4;
}
.post-body h1, 
.post-body h2, 
.post-body h3, 
.post-body h4, 
.post-body h5, 
.post-body h6{
	padding:0 0 20px 0;	
	margin:0 0 20px 0;	
	border-bottom:1px dashed #ccc;
	clear: both;
	font-family:'Monda', sans-serif;
}
.post-body h1{
	font-size: 1.4em;
}
.post-body h2{
	font-size: 1.3em;
}
.post-body h3{
	font-size: 1.2em;
}
.post-body h4{
	font-size: 1.1em;
}
.post-body h5{
	font-size: 1em;
}
.post-body h6{
    font-size: 1em;
}
.post-body embed,
.post-body audio,
.post-body iframe{
	float:left;
	width:100%;
	margin:0 0 20px 0;
}
.post-body iframe{
	min-height:450px;
}
.post-body ol{
	padding-left:60px;
	margin:0 0 20px 0;	
}
.post-body ul{
	list-style:none;
	padding-left:30px;
	margin:0 0 20px 0;	
}
@media screen and (max-width: 639px) {
.post-body ul{
	padding-left:0;
  }
}
.post-body ul li:before{
	content:'✓';
	color:#1375C6;
	vertical-align:bottom;
	padding-right:10px;
}
.post-body blockquote{
	float:left;
	width:100%;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	padding:40px;
	margin:20px 0;
	position:relative;
	color:#8c8c8c;
	font-style:italic;
	background:rgba(255,255,255,0.3);
	border:1px solid #ddd;
}
.post-body blockquote:before{
    position: absolute;
    width: 50px;
    height: 50px;
    background:#ddd;
    content: "❝";
    font-size: 30px;
    top: 0;
    left: 50%;
    margin: -25px 0 0 -25px;
    border-radius: 50%;
    text-align:center;
    line-height:55px;
    color:#3BA2F7;
    font-style:normal;
}
.post-body cite{
	float:left;
	width:100%;
	text-align:right;
	font-size:0.9em;
	margin:0 0 20px 0;
}
.post-body cite:before{
	content:'―';
}
.post-body table{
    table-layout:fixed;
    width:100%;
}
table.tr-caption-container {
     padding:0!important;
     margin-bottom: 20px!important;
}
.post-body img{
	margin-bottom:20px;
	padding:10px;
	background:#fafafa;
	border:1px solid #fff;
	box-shadow:0 1px 1px rgba(0,0,0,0.15);
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.post-body td.tr-caption{
	font-family:'Monda', sans-serif;
	text-transform:uppercase;
	letter-spacing:0.1em;
	font-size:0.7em;
}
.post-body form{
	float:left;
	width:100%;
	margin:0 0 20px 0;
}
.post-body input[type='text'],
.post-body input[type='email'],
.post-body input[type='password'],
.post-body textarea{
	float:left;
	width:100%;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
	border:1px solid #fff;
	background:#fafafa;
	box-shadow:0 1px 1px rgba(0,0,0,0.1);
	padding:20px;
	margin:0 0 25px 0;
	border-radius:0;
	-webkit-appearance:none;
    -webkit-border-radius:0px;
    -webkit-appearance:caret; 
	font-size:0.9em;
	color:#356793;
}
.post-body label{
	width:100%;
	float:left;
	padding-bottom:10px;
	color:#5B5757;
	font-family:'Monda', sans-serif;
	text-transform:uppercase;
	font-size:0.7em;
}
.asterisk{
	color:#FF6681;
	padding-left:4px;
}
.post-body input[type='submit'],
.post-body input[type='button']{
	display:table;
	margin:0 auto;
	background:#356793;
	border:1px solid #fff;
	box-shadow:0 1px 1px rgba(0,0,0,0.2);
	padding:10px;
	cursor:pointer;
	border-radius:0;
	-webkit-appearance:none;
    -webkit-border-radius:0px;
    -webkit-appearance:caret; 
	position:relative;
	font-family:'Monda', sans-serif;
	letter-spacing:0.1em;
	color:#fff;
	text-transform:uppercase;
	font-size:0.7em;
}
.post-body input[type='submit']:hover,
.post-body input[type='submit']:focus,
.post-body input[type='button']:hover,
.post-body input[type='button']:focus{
	top:2px;
}
.post-body .video-container {
	padding-bottom: 58%!important;
}
/* ------------------------------------------------------------------------------------
--  READ MORE BUTTON FOR POST
------------------------------------------------------------------------------------ */
.jump-link{
	float:left;
	width:96%;
	padding:20px 4% 0 0;
    background:#070605 url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQIW2NgYGB4z4AAFUhsFAG4IsICMIBiLgBmEQcEyASpFQAAAABJRU5ErkJggg==);
}
.jump-link a{
	float:right;
	display:inline-block;
	font-family:'Monda', sans-serif;
	font-size:0.6em;
	letter-spacing:0.2em;	
	text-transform:uppercase;
}
.jump-link a:hover{
	padding: 0 20px 0 0;
}
.jump-link span{
	display:inline-block;
	width:24px;
	height:24px;
	line-height:24px;
	border:1px solid #3BA2F7;
	text-align:center;
	margin:0 0 0 10px;
}
/* ------------------------------------------------------------------------------------
--  POST BLOCK: FOOTER
------------------------------------------------------------------------------------ */
/*-----------blogger class starts-----------*/
.post-footer{
	float:left;
	width:96%;
    border-bottom:8px solid #181511;
    margin:0 4% 0 0;
}
@media screen and (max-width: 799px) {
.post-footer{
	width:100%;
	margin:0;
}
}
.post-footer-wrap{
	float:left;
	width:100%;
	padding:30px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.post-footer-line{
	float:left;
	width:100%;
	line-height:1.7em;
	font-family:'Monda', sans-serif;
    font-size:0.8em;
}
.post-footer-line span{
	font-family:'Monda', sans-serif;
}
.post-footer-line a{
	font-family:'Monda', sans-serif;
	text-transform:uppercase;
}
/* ------------------------------------------------------------------------------------
--  post: inline ads
------------------------------------------------------------------------------------ */
.inline-ad{
	float:left;
	width:100%;
    background: #070605;
}
.inline-ad iframe{
	float:none;
	padding:0!important;
	border:20px solid transparent;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
/* ------------------------------------------------------------------------------------
--  post: labels (tags)
------------------------------------------------------------------------------------ */
.post-labels a{
	display:inline-block;
    padding:0 5px 0 0;
}
/* ------------------------------------------------------------------------------------
--  post: share buttons
------------------------------------------------------------------------------------ */
.post-share-buttons{
	float:left;
	width:100%;
	margin:10px 0;
}
/*-----------blogger class ends-----------*/
/* ------------------------------------------------------------------------------------
--  POST BLOCK: COMMENTS
------------------------------------------------------------------------------------ */
/*-----------blogger class starts-----------*/
.comments{
	float:left;
	width:100%;
	background:#070605;
    border-bottom:8px solid #356793;
    margin:0 0 30px 0 !important;
	padding:30px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.comments .comments-content{
	float:left;
	width:100%;
	background:#fff;
    margin-bottom: 0!important;
}
.comments .comments-content iframe{
	float:left;
	width:100%!important;
	padding:0!important;
	margin:0!important;
	border:20px solid #f0f0f0;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.comments h4{
	display:table;
	margin:0 auto 30px auto;
	padding:10px;
	border:1px solid #3BA2F7;
	text-transform:uppercase;
	font-family:'Monda', sans-serif;
	font-size:0.9em;
	text-align:center;
}
.comment-form{
	float:left;
	width:100%;
	background:#fff;
}
.comments .comment-form iframe{
	float:left;
	width:100%!important;
	padding:0!important;
	margin:0!important;
	border:20px solid #f0f0f0;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.comments .comment-form h4{
	display:table;
	margin:30px auto;
	padding:10px;
	border:1px solid #3BA2F7;
	text-transform:uppercase;
	font-family:'Monda', sans-serif;
	font-size:0.9em;
	text-align:center;
}
.comments .comment-form p{
	padding:20px;
	font-size:0.9em;
	line-height:1.4em;
}
li.comment{
	float:left;
	width:96%;
	padding:2%;
	background:#f0f0f0;
}
.comment-block{
	background:#fafafa;
	padding:2%;
	margin:0;
}
.continue a, 
.secondary-text a, 
.comment-thread a{
	text-transform:uppercase;
	font-family:'Monda', sans-serif;
	font-size:0.85em;
	display:inline-block;
	margin:0;
	padding:0;
}
#comments h4{
	color:#4A80AF;
}
.comment-actions a{
	display:inline-block;
	padding-right:5px;
}
.comments .comments-content .loadmore {
    margin-top: 0em!important;
    max-height: 0em!important;
    padding:10px 0;
}
.avatar-comment-indent{
	float:left;
    margin-left: 0!important;
    position: relative;
	width:100% !important;
}
.avatar-image-container,
.avatar-image-container img{
	max-width:45px !important;
	width:45px !important;
	max-height:45px !important;
	height:45px !important;
	padding: 0 !important;
	border:none !important;
}
.comments dd, .comments dt{
	background:#f0f0f0;
}
dd.comment-body{
	padding:10px 2%;
}
dt.blog-author, dt.comment-author{
	font-size:0.9em;
	padding:10px 2% 0 2%;
}
dd.comment-footer{
	margin-bottom:30px;
	font-size:0.9em;
	padding:0 2% 10px 2%;
	border-bottom:1px solid rgba(221,221,221,0.6);
}
dd.comment-footer:last-child{
	border-bottom:none;
	margin-bottom:0;
}
p.comment-footer a{
	color:#356793;
	text-transform:uppercase;
	font-family:'Monda', sans-serif;
	font-size:0.8em;
	padding-bottom:20px;
	float:left;
}
.comments .continue {
	float:left;
	width:100%;
	padding:10px 30px 30px 30px;
	box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-box-sizing:border-box;
}
.comments .continue a {
   padding: 0!important;
}
/* ------------------------------------------------------------------------------------
--  PAGER (NEXT PREVIOUS BUTTONS)
------------------------------------------------------------------------------------ */
.blog-pager-menu{
	float:left;
	width:100%;
	margin:0 0 20px 0;
}
.blog-pager-menu ul{
	list-style:none;
	margin:0 auto;
	display:table;
}
.blog-pager-menu li{
	float:left;
	margin-bottom:5px;
}
.blog-pager-menu a{
	display:inline-block;
	padding:10px 14px;
	margin:0 5px 0 0;
	color:#aaa;
	text-transform:uppercase;
	font-size:0.7em;
	letter-spacing:0.1em;
	color:#b1b1b1;
	border:1px solid rgba(255,255,255,0.1);
	font-weight:700;
}
.blog-pager-menu a:hover{
    color:#7baad4;
}
/* ------------------------------------------------------------------------------------
--  STATUS-MESSAGE
------------------------------------------------------------------------------------ */
.status-msg-wrap-custom{
    float:left;
	padding:2% 0;
	width:100%;
    background:#070605;
    border-bottom:8px solid #181511;
    margin-bottom:20px;
}
.status-msg-wrap-custom a{
	padding:0 6px;
	text-transform:uppercase;
}
.status-msg-wrap-custom b{
	text-transform:uppercase;
}
.status-msg-body-custom{
	padding:0 4%;
	font-family:'Monda', sans-serif;
	font-size:0.85em;
}
/* ------------------------------------------------------------------------------------
--  FEED LINKS
------------------------------------------------------------------------------------ */
.feed-links{
	text-align:center;
	margin-bottom:10px;
}
/*-----------blogger class ends-----------*/
/* ------------------------------------------------------------------------------------
--  WIDGETS
------------------------------------------------------------------------------------ */
/* ------------------------------------------------------------------------------------
--  WIDGETS FOR SIDEBAR 
------------------------------------------------------------------------------------ */
.sidebar .widget:last-child{
	margin-bottom:0;
}
#sidebar-box h2,
.sidebar .widget h2{
	letter-spacing:0.1em;
	margin-bottom:20px;
	text-transform:uppercase;
	color:#565656;
	font-family:'Oswald', sans-serif;
	line-height:1.5em;
    background:rgba(227,227,227,0.7) url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAAECAQAAADl0Z2xAAAAEElEQVQIHWNgYGD4b8UABgAJmgE6cUJg+wAAAABJRU5ErkJggg==);
    padding:3%;
}
.sidebar .widget .readmore{
	margin-top:10px;
}
.sidebar ul,
.sidebar ol{
	float:left;
	width:100%;	
	font-family:'Monda', sans-serif;
	font-size:1.1em;	
}
.sidebar ul, .sidebar ol{
	list-style:none;	
}
.sidebar .widget li{
	margin-bottom:0.8em;
	line-height:1.5em;	
	padding-bottom:10px;
	border-bottom:1px solid rgba(192,192,192,0.6);/*#c0c0c0*/
}
.sidebar .widget li a, 
.sidebar .widget li span{
	text-transform:capitalize;		
}
/* ------------------------------------------------------------------------------------
--  LABELS
------------------------------------------------------------------------------------ */
.sidebar .Label li:before{
	content:'✓';
	margin:0 10px 0 0;
	font-size:14px;
	border-radius:50%;
    background:#356793;
	width:24px;
	height:24px;
	display:inline-block;
	text-align:center;
	color:#fff;
	border:4px solid #fff;
	box-shadow:0 1px 1px rgba(0,0,0,0.1);
}
.sidebar .widget,
.search .widget{
	float:left;
	width:100%;
	font-size:0.9em;
	margin-bottom:30px;
}
/* ------------------------------------------------------------------------------------
--  ABOUT ME
------------------------------------------------------------------------------------ */
dl.profile-datablock {
    margin: 0!important;
}
dt.profile-data a{
	padding-top:0;
    line-height:normal;
	font-size:0.9em;
}
/* ------------------------------------------------------------------------------------
--  DEFAULT BLOG ARCHIVE
------------------------------------------------------------------------------------ */
.zippy-custom{
	color:#356793;
	font-size:0.8em;
}
/* ------------------------------------------------------------------------------------
--  POPULAR POSTS
------------------------------------------------------------------------------------ */
.sidebar .item-title{
	text-transform:capitalize;
}
.sidebar .item-snippet{
	font-size:0.9em;
	overflow:hidden;
}
@media screen and (max-width: 1279px) {
.sidebar .item-snippet{
	overflow:visible;
  }
}
/* ------------------------------------------------------------------------------------
--  IMAGE
------------------------------------------------------------------------------------ */
.sidebar .Image{
	float:left;
	width:100%;
	padding:20px;
	box-sizing:border-box;
	-webkit-box-sizing:border-box;
	-moz-box-sizing:border-box;
	border:1px solid #fff;
	background:#f0f0f0;
	box-shadow:0 1px 1px rgba(0,0,0,0.2);	
}
.sidebar .Image .caption{
	float:left;
	width:100%;
	text-transform:uppercase;
	letter-spacing:0.1em;
	font-family:'Monda', sans-serif;
	font-size:0.8em;
	text-align:center;
}
/* ------------------------------------------------------------------------------------
--  ADSENSE 
------------------------------------------------------------------------------------ */
.adsense-wrap{
	float:left;
	width:100%;
	padding:20px;
	box-sizing:border-box;
	-webkit-box-sizing:border-box;
	-moz-box-sizing:border-box;
	border:1px solid #fff;
	background:#f0f0f0;
	box-shadow:0 1px 1px rgba(0,0,0,0.2);
}
.sidebar .widget figure{
	margin:0 auto;
	display:table;
}
/* ------------------------------------------------------------------------------------
--  FOLLOW BY EMAIL (#FollowByEmail1) + CUSTOM SEARCH 
------------------------------------------------------------------------------------ */
.search{
	float:left;
	width:100%;
	margin:30px 0 0 0;
}
.sidebar .widget form,
.search .widget form{
    float:left;
    width:100%;
    clear:both;	
}
.sidebar .widget form input,
.search .widget form input{	
	font-family:'Monda', sans-serif;
	text-transform:uppercase;
}
.inputfield{
	float:left;
	background:#f0f0f0;
	color:#bebebe;
	width:57%;
    padding:0 2%;
	border:none;
	border-bottom:1px solid #bebebe;
	height:36px;
	outline:none;
}
.submitbutton{
	float:right;
	width:36%;
	height:36px;
	background:#356793;
	box-shadow: 0 1px 4px rgba(0,0,0,0.2);
	border:1px solid rgba(255,255,255,0.1);
    color:#fff;
    font-size:0.8em;
	letter-spacing:0.1em;
	cursor:pointer;
    -moz-transition: 500ms ease-in;
    -o-transition: 500ms ease-in;
    -webkit-transition: 500ms ease-in;
    -ms-transition: 500ms ease-in;
    transition: 500ms ease-in; 
}
.submitbutton:hover{
	background:#070605;
}
/* ------------------------------------------------------------------------------------
--  LINK TO ARCHIVE PAGE (#HTML3)
------------------------------------------------------------------------------------ */
.readmore{
	float:left;
	width:98%;
	padding:1%;
    background:rgba(227,227,227,0.7) url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAAECAQAAADl0Z2xAAAAEElEQVQIHWNgYGD4b8UABgAJmgE6cUJg+wAAAABJRU5ErkJggg==);
}
.readmore a{
	float:right;
	display:block;
	color:#214b70;	
	font-family:'Monda', sans-serif;
	text-transform:capitalize;
}
.readmore a:hover{
	padding: 0 20px 0 0;
	color:#3BA2F7;
}
.readmore a span{
    opacity: 0;
    filter: alpha(opacity = 0);	
}
.readmore a:hover span{
    opacity: 0.95;
    filter: alpha(opacity = 95);
}
/* ------------------------------------------------------------------------------------
--  STATISTICS (#Stats1)
------------------------------------------------------------------------------------ */
.Stats{
	float:left;
	width:100%;
}
.Stats .widget-content{
	float:left;
	width:100%;	
}
.Stats #Stats1_content{
    display: table!important;
    margin:0 auto;	
}
.Stats #Stats1_content span.text-counter-wrapper{
    padding:0 8px 5px 8px;
	background:#356793;
	box-shadow:inset 0 0 4px rgba(0,0,0,0.2);
	border:1px solid rgba(255,255,255,0.1);
    color:#fff;
    font-size: 18px!important;
    font-weight:lighter!important;
}
/* ------------------------------------------------------------------------------------
--  HOME PAGE
------------------------------------------------------------------------------------ */
#highlight{
	float:left;
	width:100%;
	background:transparent;
	position:relative;
}
#main1{
	float:left;
	width:100%;	
}
/* ------------------------------------------------------------------------------------
--  HOME PAGE WIDGET IMAGE + POPULAR POSTS
------------------------------------------------------------------------------------ */
#main1 h2{
	display:none;
}
#main1 .Image{
	float:left;
	width:100%;
	background:transparent;
}
#main1 .Image img{
	-webkit-filter:saturate(110%);
}
#main .Image .caption{
	display:none;
}
#main1 .PopularPosts{
	position:absolute;
	top:40px;
	left:40px;
	width:100%;
}
#main1 .PopularPosts ul{
	float:left;
	width:55%;
	display:inline-block;
	padding:20px;
	background:rgba(0, 0, 0, 0.8);
	box-shadow:0 1px 100px #000;
	border:1px solid rgba(255,255,255,0.05);
	list-style:none;
	box-sizing:border-box;
	-webkit-box-sizing:border-box;
	-moz-box-sizing:border-box;
	-webkit-animation-delay:4s;
	 animation-delay:4s;
}
@media screen and (max-width: 1280px) {
#main1 .PopularPosts ul{
	width:60%;
  }
}
@media screen and (max-width: 1279px) {
#main1 .PopularPosts ul{
	width:70%;
  }
}
@media screen and (max-width: 799px) {
#main1 .PopularPosts ul{
	display:none;
  }
}
#main1 .PopularPosts ul li{
	float:left;
	width:100%;
	text-align:center;
}
#main1 .PopularPosts .item-title{
    padding-bottom: 0!important;
}
#main1 .PopularPosts a{
	color:#aaa;
	font-family:'Oswald', sans-serif;
	font-size:0.9em;
	letter-spacing:0.1em;
	text-transform:uppercase;
	line-height:1.6em;
	overflow:hidden;
}
#main1 .PopularPosts a:hover,
#main1 .PopularPosts a:focus{
	color:#356793
}
#main1 .PopularPosts .item-snippet{
    margin:10px 0 0 0;
    line-height:1.4em;
	overflow:hidden;
}
#main1 .PopularPosts img{
	-webkit-filter:saturate(140%);
}
/* ------------------------------------------------------------------------------------
--  HOME PAGE GALLERY (IMAGE WIDGET)
------------------------------------------------------------------------------------ */
#gallery{
	float:left;
	width:100%;
}
.image-row-text{
	float:left;
	width:100%;
	margin:20px 0;
	text-align:center;
}
.image-row-text h4{
	font-size:1.2em;	
	letter-spacing:0.1em;
	color:#1375c6;	
	font-family: 'Monda', sans-serif;
	text-transform:uppercase;
	line-height:1.2em;
}
#main3{
    padding:1%;
    clear: both;
    margin-bottom:10px;
}
@media screen and (max-width: 1023px) {
#main3{
	float:left;
	position:relative;
    width:100%;
    padding:0;
	box-sizing:border-box;
	-webkit-box-sizing:border-box;
	-moz-box-sizing:border-box;
	border:20px solid transparent;
  }
}
#main3 h2{
	display:none;
}
#main3 .Image{
    float: left;
    width:28.6%;
    margin: 1%;
    padding: 1%;
	background:rgba(0,0,0,0.4);	
}
@media screen and (max-width: 1366px) {
#main3 .Image{
    width:28%;
  }
}
@media screen and (max-width: 1023px) {
#main3 .Image{
    width:100%;
    margin:0;
    padding:0;
  }
}
#main3 .Image img{
     width:100%;
     max-width:100%;
     height:auto; 
}
#main3 .Image .caption{
	float:left;
	width:100%;
	text-transform:uppercase;
	letter-spacing:0.1em;
	font-family:'Monda', sans-serif;
	font-size:0.7em;
	text-align:center;
	margin:0 0 14px 0;
}
@media screen and (max-width: 1023px) {
#main3 .Image .caption{
	margin:0 0 20px 0;
  }
}
#main3 .widget-content{
	float:left;
	width:100%;
	background:#111;
	box-shadow:0 1px 20px #000;
	border:1px solid rgba(255,255,255,0.07);	
	box-sizing:border-box;
	-webkit-box-sizing:border-box;
	-moz-box-sizing:border-box;
	padding:20px 20px 0 20px;
}
@media screen and (max-width: 1023px) {
#main3 .widget-content{
	box-shadow:none;
	padding:0;
	border:none;
	background:transparent;
}
}
.transitions-enabled.masonry,
.transitions-enabled.masonry .masonry-brick {
  -webkit-transition-duration: 0.7s;
     -moz-transition-duration: 0.7s;
      -ms-transition-duration: 0.7s;
       -o-transition-duration: 0.7s;
          transition-duration: 0.7s;
}
.transitions-enabled.masonry {
  -webkit-transition-property: height, width;
     -moz-transition-property: height, width;
      -ms-transition-property: height, width;
       -o-transition-property: height, width;
          transition-property: height, width;
}
.transitions-enabled.masonry  .masonry-brick {
  -webkit-transition-property: left, right, top;
     -moz-transition-property: left, right, top;
      -ms-transition-property: left, right, top;
       -o-transition-property: left, right, top;
          transition-property: left, right, top;
}
/* ------------------------------------------------------------------------------------
--  STATIC PAGES
------------------------------------------------------------------------------------ */
/* ------------------------------------------------------------------------------------
--  STATIC PAGES: ARCHIVE PAGE
------------------------------------------------------------------------------------ */
.archives, .archives a{
	float:left;
	width:100%;
}
.archives p{
	margin-bottom:0;
	padding:2% 2% 0 2%;
}
.archive-item{
	float:left;
	width:100%;	
	margin-bottom:20px;
	border-bottom:1px solid rgba(255,255,255,0.7);
    background:rgba(255,255,255,0.3);
}
.archive-item:last-child{
	margin-bottom:0;
}
.archive-single{
	float:left;
	width:100%;
	padding-bottom:2%;
	border-bottom:1px solid #ddd;
}
.archive-single p{
	text-transform:capitalize;
}
/* ------------------------------------------------------------------------------------
--  ERROR PAGE
------------------------------------------------------------------------------------ */
#error-page{
    float:left;
    width:100%;
	text-align:center;
	margin:20px 0 0 0;
}
#error-404{ 
	margin:0 auto;
	width:240px;
	height: 240px; 
	border: 20px solid #1B1B1B; 
	border-radius: 240px; 
	-moz-transition: 500ms ease-in;
    -o-transition: 500ms ease-in;
    -webkit-transition: 500ms ease-in;
    -ms-transition: 500ms ease-in;
    transition: 500ms ease-in; 	
}
#error-404:hover{ 
	border-color: #333;
}
#error-404 span{ 
	color:#3BA2F7;
	font-size: 100px; 
	font-weight: bold; 
	line-height: 240px; 
} 
#error-page hgroup{
	margin:30px 0 0 0;
}
#error-page h1{
	text-transform:capitalize;
	font-size:2em;
	margin-bottom:20px;
}
#error-page h2{
	font-size:1.2em;
}
/* ------------------------------------------------------------------------------------
--  FOOTER
------------------------------------------------------------------------------------ */
footer{
	float:left;
	width:100%;
	text-align:center;
	margin-bottom:40px;
}
footer small{
	font-size:0.8em;
	font-family:'Monda', sans-serif;
	color:#aaa;
	background:rgba(0,0,0,0.4);
	padding:4px;
	display:inline-block;
}
footer a{
	color:#356793;
}
footer a:hover,
footer a:focus{
    color:#4a80af;
}
