# PoemWebsite
<html>
<link rel ="stylesheet" type="text/css" href="css/stylesheet.css">
</head>
<body>
<header>
<div class="main">
<div class="logo">
<img src="lo.jfif" width =80 height=80>
<ul>
<li><a href ="home.html">Home</a></li>
<li><a href ="category.html">Category</a></li>
<li><a href ="SignUp.html">Signup</a></li>
</ul>
</div>
<div class ="sign-up-form">
<h1>Sign UP</h1>
<form>
<label>Full name:</label>
<input type="textfield"   name="tb1" placeholder="Full Name" id="fullname"><br>
<br>
<label> Password :</label>
<input type="password"  name="pwd"  placeholder="Password"id="pwd"><br>
<br>
<label>Address :</label>
<textarea cols="20" rows="1" placeholder="Address" ></textarea><br><br>
<br>
<label>Gender :</label>
<input type="radio"name="rb1">MALE
<input type="radio"name="rb1">FEMALE<br>
<br>

<button onclick="myFunction()">Sign up</button>

<p id="demo"></p>

<script>
function myFunction() {
  var txt;
  if (confirm("You Have Signed in")) {
    txt = "You Have Signed in";
  }
else{
  txt="You have not sign in";
  }
  document.getElementById("demo").innerHTML = txt;
}
</script>
</form>
</body>
</html>
</div>
</div>
</div>
</header>
</body>
</html>
</html> 
 BIN +28.9 KB 
book.jpg

 80  
category.html
@@ -0,0 +1,80 @@
<html>
<head>
<link rel ="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
<header>
<div class="main">
<div class="logo">
<img src="lo.jfif" width =80 height=80>
<ul>
<li><a href ="home.html">Home</a></li>
<li><a href ="category.html">Category</a></li>
<li><a href ="SignUp.html">Signup</a></li>
</ul>
<h1>Category</h1>
<br>
<br>
<style>
div.gallery {
  margin: 5px;
  border: 1px solid grey;
  float: left;
  width: 200px;
  height: 200px; 
}

div.gallery:hover {
  border: 1px solid #fff;
}

div.gallery img {
  width: 100%;
  height: 80%;
}

div.desc {
  padding: 6px;
  text-align: center;
  color: #fff;
}
div.head{
   text-align: center;
</style>
</head>
<body>

<div class="gallery">
  <a target="_blank" href="inspirational poems.jpg">
    <img src="ip.jpg" alt="Inspiration poems" >
  </a>
  <div class="desc">All Inspiring ones are here displayed </div>
</div>

<div class="gallery">
  <a target="_blank" href="images.jfif">
    <img src="images.jfif" alt="childern poems" width="600" height="400">
  </a>
  <div class="desc">Poems for age group 8 to12</div>
</div>

<div class="gallery">
  <a target="_blank" href="np.jpg">
    <img src="np.jpg" alt="Nature poems" width="600" height="400">
  </a>
  <div class="desc">Beautifull poems about nature</div>
</div>

<div class="gallery">
  <a target="_blank" href="rp.jpg">
    <img src="rp.jpg" alt="Rhymming poems">
  </a>
  <div class="desc">Great Rhymming poems are here</div>
</div>
.<div class="head">
</div>
</div>
</div>
</header>
</body>
</html> 
 40  
css/style.css
@@ -0,0 +1,40 @@
{
padding:0;
margin:0;
font-family:' Josefin Sans,sans-serif';
box-sizing:bordrer-box;
}
.logo{
margin:left;
border-radius: 80px;
}
header {
              background-image: url(../gh.png );
             height:100%;
             background-size:cover;
             background-position:center;

}
ul{
float:right;
list-style-type:none;
}
h1{
text-align: center;
color:white;
}
ul li{
display:inline-block;
}
ul li a{
text-decoration:none;
color:white;
padding:5px 20px;
border:1px solid grey;
transition: 0.6ease;
justify-content:space-around;
}
ul li a:hover{
background-color: #fff;
color:#000;
} 
 59  
css/stylesheet.css
@@ -0,0 +1,59 @@
{
margin:0;
padding:0;
}
header {
              background-image: url(../book.jpg );
             height:100%;
             background-size:cover;
             background-position:center;

}
ul{
float:right;
list-style-type:none;
top: 100px;
}
ul li{
display:inline-block;
}
ul li a{
text-decoration:none;
color:#fff;
padding:5px 20px;
border:1px solid white;
transition: 0.6ease;
}
ul li a:hover{
background-color: #fff;
color:#000;
}
.title{
position:absolute;
top:50%;
left:50%;
transform:translate(-50%,-50%);
}
.title h1{
color:#fff;
}
.sign-up-form{
width:300px;
font-size:14px;
border radius:10px;
box-shadow:0 0 3px 0 rgba(0,0,0,0.5);
background-color:rgba(0,0,0,0.5);
color:#fff;
padding:0px;
margin:8% auto 0;
text-allign:center;
}
form#signup{
     margin: 40px; 
}
p{
color:#fff;
}



 BIN +2.62 MB 
gh.png

 29  
home.html
@@ -0,0 +1,29 @@
<html>
<head>
<title> Poems Website </title>
<link rel ="stylesheet" type="text/css" href="css/stylesheet.css">
</head>
<body>
<header>
<div class="main">
<div class="logo">
   <img src="lo.jfif" width=80px height=80px >
<ul>
<li><a href =#>Home</a></li>
<li><a href ="category.html">Category</a></li>
<li><a href ="SignUp.html">Signup</a></li>
</ul>
<div class ="title">
<h1> World Of Poems</h1>
<p>Experience different types of poems in the world of poems . A new different era for poems organised and designed for user friendly interface</p>
<p id="demo" style="display:none">Welcome to the interface!!!</p>

<button type="button" onclick="document.getElementById('demo').style.display='block'">Click Me!</button>
<button type="button" onclick="document.getElementById('demo').style.display='none'">Hide!</button>

</div>
</div>
</div>
</header>
</body>
</html> 
 BIN +14.9 KB 
images.jfif
Binary file not shown.
 BIN +267 KB 
ip.jpg

 BIN +29.3 KB 
lo.jfif
Binary file not shown.
 BIN +564 KB 
np.jpg

 BIN +39.2 KB 
rp.jpg

 40  
style.css
@@ -0,0 +1,40 @@
{
padding:0;
margin:0;
font-family:' Josefin Sans,sans-serif';
box-sizing:bordrer-box;
}
.logo{
margin:left;
border-radius: 80px;
}
header {
              background-image: url(../gh.png );
             height:100%;
             background-size:cover;
             background-position:center;

}
ul{
float:right;
list-style-type:none;
}
h1{
text-align: center;
color:white;
}
ul li{
display:inline-block;
}
ul li a{
text-decoration:none;
color:white;
padding:5px 20px;
border:1px solid grey;
transition: 0.6ease;
justify-content:space-around;
}
ul li a:hover{
background-color: #fff;
color:#000;
} 
