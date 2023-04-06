<script>
// @ts-nocheck

 let slideIndex = 0;
 export let images = [];

 function showSlides() {
   let i;
   const slides = document.getElementsByClassName("slider-image");
   const dots = document.getElementsByClassName("slider-dot");
   for (i = 0; i < slides.length; i++) {
     slides[i].style.display = "none";
   }
   slideIndex++;
   if (slideIndex > slides.length) {
     slideIndex = 1;
   }
   for (i = 0; i < dots.length; i++) {
     dots[i].className = dots[i].className.replace(" active", "");
   }
   slides[slideIndex - 1].style.display = "block";
   dots[slideIndex - 1].className += " active";
   setTimeout(showSlides, 10000);
 }

 showSlides();
</script>

<div class="slider-container relative overflow-hidden">
 <div class="slider-wrapper flex">
   {#each images as image}
     <img src={image.src} alt={image.alt} class="slider-image w-full h-full object-cover">
   {/each}
 </div>
 <div class="slider-navigation absolute bottom-0 right-0 z-10">
   <div class="slider-dots">
     {#each images as _, i}
       <span class="slider-dot" onclick={() => slideIndex = i}></span>
     {/each}
   </div>
   <div class="slider-arrows">
     <button class="slider-arrow left-0" onclick={() => slideIndex -= 1}>&lt;</button>
     <button class="slider-arrow right-0" onclick={() => slideIndex += 1}>&gt;</button>
   </div>
 </div>
</div>


