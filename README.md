### <html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial;
  margin: 0;
}
.background{
  background-color: background-color: #000000;
background-image: linear-gradient(147deg, #000000 0%, #04619f 74%);
}
* {
  box-sizing: border-Box;
}

img {
  vertical-align: middle;
}
img{
  object-fit: scale-down;
}

/* Position the image container (needed to position the left and right arrows) */
.container {
  position: relative;
}

/* Hide the images by default */
.mySlides {
  display: none;
}

/* Add a pointer when hovering over the thumbnail images */
.cursor {
  cursor: pointer;
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
  position:fixed;
  top: 40%;
  width: auto;
  padding: 16px;
  margin-top: -50px;
  color: white;
  font-weight: bold;
  font-size: 20px;
  border-radius: 0 3px 3px 0;
  user-select: none;
  -webkit-user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* Container for image text */
.caption-container {
  text-align: center;
  background-color: #222;
  padding: 2px 16px;
  color: white;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Six columns side by side */
.column {
  float: left;
  width: 16.66%;
}

/* Add a transparency effect for thumnbail images */
.demo {
  opacity: 0.6;
}

.active,
.demo:hover {
  opacity: 1;
}
</style>
<body>
  <div class="background">

<h2 style="text-align:center">Avengers Gallery</h2>

<div class="container">
  <div class="mySlides">
    <div class="numbertext">1 / 6</div>
    <img src="ironman.jpg" style="width:100%" >
    </div>
   </div>

  <div class="mySlides">
    <div class="numbertext">2 / 6</div>
    <img src="captain america.jpg" style="width:100%">
  </div>

>
  <div class="mySlides">
    <div class="numbertext">3 / 6</div>
    <img src="thor.jpg" style="width:100%">
  </div>

>
  <div class="mySlides">
    <div class="numbertext">4 / 6</div>
    <img src="hulk.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">5 / 6</div>
    <img src="doctor strange.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">6 / 6</div>
    <img src="spider man.jpg" style="width:100%">
  </div>
</div>

  <a class="prev" onclick="plusSlides(-1)">???</a>
  <a class="next" onclick="plusSlides(1)">???</a>

  <div class="caption-container">
    <p id="caption"></p>
  </div>
  <div class="background">

  <div class="row">
    <div class="column">
      <img class="demo cursor" src="ironman.jpg" style="width:100%" onclick="currentSlide(1)" alt="ironman">
    </div>
    <div class="column">
      <img class="demo cursor" src="captain america.jpg" style="width:100%" onclick="currentSlide(2)" alt="Captain america">
    </div>
    <div class="column">
      <img class="demo cursor" src="thor.jpg" style="width:100%" onclick="currentSlide(3)" alt="thor">
    </div>
    <div class="column">
      <img class="demo cursor" src="hulk.jpg" style="width:100%" onclick="currentSlide(4)" alt="hulk">
    </div>
    <div class="column">
      <img class="demo cursor" src="doctor strange.jpg" style="width:100%" onclick="currentSlide(5)" alt="doctor strange">
    </div>
    <div class="column">
      <img class="demo cursor" src="spider man.jpg" style="width:100%" onclick="currentSlide(6)" alt="Spiderman">
    </div>
  </div>
</div>
</div>

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  var captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>

</body>
</html>

<!--
**Ish1u/Ish1u** is a ??? _special_ ??? repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- ???? I???m currently working on ...
- ???? I???m currently learning ...
- ???? I???m looking to collaborate on ...
- ???? I???m looking for help with ...
- ???? Ask me about ...
- ???? How to reach me: ...
- ???? Pronouns: ...
- ??? Fun fact: ...
-->
