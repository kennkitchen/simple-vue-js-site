<template>
  <div id="main" class="home">

    <MenuOpen></MenuOpen>

    <div class="w3-container">
      <h1>Home</h1>
      <p>In this example, the sidebar is hidden (style="display:none")</p>
      <p>It is shown when you click on the menu icon in the top left corner.</p>
      <p>When it is opened, it shifts the page content to the right.</p>
      <p>We use JavaScript to add a 25% left margin to the div element with id="main" when this happens. The value "25%" matches the width of the sidebar.</p>
    </div>

  </div>
</template>

<script>

import MenuOpen from "@/components/MenuOpen";
export default {
  name: 'HomeView',
  components: {MenuOpen},
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
