<template>
  <div id="main" class="home">
    <div class="w3-container">
      <h1>Home</h1>
      <p>This is the home page.</p>
      <p>This is a site built with Vue.js that I'm using as a personal refresher.</p>
      <p>As you can see, there isn't a lot here yet! And, chances are, I'll break it a few times before it gets better.</p>
      <WeatherData v-bind:weather="weather"></WeatherData>
    </div>
  </div>
</template>

<script>

import WeatherData from "@/components/WeatherData.vue";
export default {
  name: 'HomeView',
  components: {WeatherData},
  // methods: {
  //   w3Open() {
  //     document.getElementById("main").style.marginLeft = "25%";
  //     document.getElementById("mySidebar").style.width = "25%";
  //     document.getElementById("mySidebar").style.display = "block";
  //     document.getElementById("openNav").style.display = 'none';
  //   }
  // }

}
</script>
