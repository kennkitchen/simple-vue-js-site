<template>
  <div class="w3-indigo">
    <button id="openNav" class="w3-button w3-indigo w3-xlarge" @click="w3Open">&#9776;</button>
  </div>
</template>

<script>
export default {
  name: 'MenuOpen',
  // props: {
  //   title: String
  // }
  methods: {
    w3Open() {
      document.getElementById("main").style.marginLeft = "25%";
      document.getElementById("mySidebar").style.width = "25%";
      document.getElementById("mySidebar").style.display = "block";
      document.getElementById("openNav").style.display = 'none';
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
