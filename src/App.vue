<script setup>


</script>

<template>
  
  <header>
  
    <ul class="snip1226">
  <li class="nav-btn current"><a href="#" data-hover="Home">Home</a></li>
  <!--<li class="nav-btn"><a href="#about" data-hover="About">About</a></li>-->
  <li class="nav-btn"><a href="#work" data-hover="Work">Work</a></li>
  <li class="nav-btn"><a href="#education" data-hover="Education">Education</a></li>
  <li class="nav-btn"><a href="#contact" data-hover="Contact">Contact</a></li>
  <li><h2>(Work in prgress)</h2></li>
  
</ul>
  </header>

  <RouterView />
</template>

<style scoped>




</style>
<script>
  document.addEventListener("DOMContentLoaded", function() {
    var btns = document.querySelectorAll(".nav-btn");

    btns.forEach(function(btn) {
      btn.addEventListener("click", function() {
        var currentActive = document.querySelector(".nav-btn.current");
        if (currentActive) {
          currentActive.classList.remove("current");
        }
        this.classList.add("current");
      });
    });
  });
</script>


