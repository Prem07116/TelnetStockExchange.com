<!DOCTYPE html>
<html lang="en">
<head>
  <title>Telnet</title>
  <link rel="stylesheet" href="body.css">
  <link rel="icon" href="file:///C:/Softwere/Img/Black%20And%20Gold%20Elegant%20Fashion%20Logo.png">
</head>
<body>
   <h1><center>
    Telnet</center>
  </h1>
  <ul>
    <li>
      <a href="file:///C:/Softwere/site/index.html"> Home </a></li>
    <li><a href="#"> Coding </a></li>
    <li><a href="file:///C:/Softwere/site/marketing.html"> Market </a></li>
    <li><a href="file:///C:/Softwere/site/contact.html"> Classes </a></li>
    <li> <a href="file:///C:/Softwere/site/about.html"> About </a> </li>
  </ul>
  
  <!-- Slideshow container  -->
  <div class="slideshow-container">
   
      <div class="mySlides fade">
        
     <center><img src="file:///C:/Softwere/Img/istockphoto-1367783784-1024x1024.jpg" style="width: 60pc; height: 500px; " ></center>
        
    </div>
    <div class="mySlides fade">
      
    <center><img src="file:///C:/Softwere/Img/istockphoto-1423664634-1024x1024.jpg" style="width: 60pc;" height="500px" ></center>
      
  </div>
  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides (-1) ">&#10094</a>
  <a class="next" onclick="plusSlides (1) ">&#10095</a>
  </div>
  <br>
  <!-- the dots/circles -->
  <div style="text-align:center;">
    <span class="dot" 
      onclick="currentSlide(1)">
    </span>
    <span class="dot" 
      onclick="currentSlide(2)"></span>
      <span class="dot" 
      onclick="currentSlide(3)"></span>
  </div>
  
</body>
<script>
  let slideIndex = 1;
showSlides(slideIndex);

// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
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
}
</script>
</html>
