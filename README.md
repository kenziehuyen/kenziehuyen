
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>kenziehuyen</title>
<style>
body {
  margin: 0;
  font-size: 22px;
  color:red; 
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  background-color: #F1E0EE ;
}
.header {
  background-color: white;
  padding: 5px;
  text-align: center;
  color: red;
  font-weight: bold;
  background-color: #F1E0EE;
}

#navbar {
  overflow: hidden;
  background-color: white;
  text-align: center;
}

#navbar a {
  float: left;
  display: block;
  color: #5498EA;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 22px;
}

#navbar a:hover {
  background-color: white;
  color: #E589E8;
}

#navbar a.active {
  background-color: white;
  
  color: #E589E8;
  font-weight: bold;
}

.content {
  padding: 16px;
}

.sticky {
  position: fixed;
  top: 0;
  width: 100%;
}

.sticky + .content {
  padding-top: 60px;
}

* {box-sizing: border-box;}
body {font-family: Verdana, sans-serif;}
.mySlides {display: none;}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active {
  background-color: #f8c4ea;
}

.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@media only screen and (max-width: 300px) {
  .text {font-size: 11px}
}
</style>
</head>
<body>
<div class="header">
  <h3>KENZIE HUYEN</h3>
</div>

<div id="navbar">
  <a class="nav-link active text-primary" aria-current="page" href="../CODE/PAGEONE.html">HOME</a>
  <a class="nav-link" href="../CODE/pictures.html">PHOTOS</a>

  <a class="nav-link" href="../CODE/contact.html">CONTACT ME</a>
</div>

<script>
window.onscroll = function() {myFunction()};

var navbar = document.getElementById("navbar");
var sticky = navbar.offsetTop;

function myFunction() {
  if (window.pageYOffset >= sticky) {
    navbar.classList.add("sticky")
  } else {
    navbar.classList.remove("sticky");
  }
}
</script>
<body>


<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 5</div>
  <img src="../images/CAR1.JPG" style="width:100%">
  <div class="text">MY FRIENDS</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 5</div>
  <img src="../images/CAR5.JPG" style="width:100%">
  <div class="text">FLYING</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 5</div>
  <img src="../images/MPLS.JPG" style="width:100%">
  <div class="text">PARENTS!</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">4 / 5</div>
  <img src="../images/CARAMS.JPG" style="width:100%">
  <div class="text">THIS IS ME</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">5 / 5</div>
  <img src="../images/CAR4.JPG" style="width:100%">
  <div class="text">FRIENDS AROUND THE TABLE</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">5 / 5</div>
  <img src="../images/PRIMO1.JPG" style="width:100%">
  <div class="text">MY FRIEND PRIMO</div>

</div>
</div>
<br>

<div style="text-align:center">
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
</div>

<script>
let slideIndex = 0;
showSlides();

function showSlides() {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
  setTimeout(showSlides, 6000); // Change image every 6 seconds
}
</script>
<p>I study New Media and Digital Design with a <br>
  concentration in Art, Text, and Design. </p>
  <h4>I enjoy working creatively with others. </h4>

</body>



</body>

