<template>
  <div class="w3-bar w3-light-grey">
    <router-link to="/" class="w3-bar-item w3-button" @click="w3Close">Home</router-link>
    <router-link to="/about" class="w3-bar-item w3-button" @click="w3Close">About</router-link>
    <router-link to="/contact" class="w3-bar-item w3-button" @click="w3Close">Contact</router-link>
    <div class="w3-dropdown-hover">
      <button class="w3-button">For Future Use</button>
      <div class="w3-dropdown-content w3-bar-block w3-card-4">
        <a href="#" class="w3-bar-item w3-button">Link 1</a>
        <a href="#" class="w3-bar-item w3-button">Link 2</a>
        <a href="#" class="w3-bar-item w3-button">Link 3</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DefaultHeader',
  // props: {
  //   title: String
  // }
  // methods: {
  //   w3Close() {
  //     document.getElementById("main").style.marginLeft = "0%";
  //     document.getElementById("mySidebar").style.display = "none";
  //     document.getElementById("openNav").style.display = "inline-block";
  //   }
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--<style scoped>-->

<!--</style>-->
