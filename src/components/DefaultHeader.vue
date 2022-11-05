<template>
  <div class="">
    <div class="w3-sidebar w3-bar-block w3-card w3-animate-left" style="display:none" id="mySidebar">
      <button class="w3-bar-item w3-button w3-large"
              @click="w3Close">Close &times;</button>
      <router-link to="/" class="w3-bar-item w3-button" @click="w3Close">Home</router-link>
      <router-link to="/about" class="w3-bar-item w3-button" @click="w3Close">About</router-link>
      <router-link to="/contact" class="w3-bar-item w3-button" @click="w3Close">Contact</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DefaultHeader',
  // props: {
  //   title: String
  // }
  methods: {
    w3Close() {
      document.getElementById("main").style.marginLeft = "0%";
      document.getElementById("mySidebar").style.display = "none";
      document.getElementById("openNav").style.display = "inline-block";
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--<style scoped>-->
<!--h3 {-->
<!--  margin: 40px 0 0;-->
<!--}-->
<!--ul {-->
<!--  list-style-type: none;-->
<!--  padding: 0;-->
<!--}-->
<!--li {-->
<!--  display: inline-block;-->
<!--  margin: 0 10px;-->
<!--}-->
<!--a {-->
<!--  color: #42b983;-->
<!--}-->
<!--</style>-->
