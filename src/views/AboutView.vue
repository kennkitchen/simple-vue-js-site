<template>
  <div id="main" class="home">
    <div class="w3-container">
      <h1>About {{ title }}</h1>
      <p>This is the about page.</p>
      <p>This is a site built with Vue.js that I'm using as a personal refresher.</p>
      <p>As you can see, there isn't a lot here yet! Mainly I'm getting re-familiarized with routing at the moment.</p>
    </div>
  </div>
</template>

<script>

// import MenuOpen from "@/components/MenuOpen";
export default {
  name: 'AboutView',
  // components: {MenuOpen},
  data() {
    return {
      title: process.env.VUE_APP_TEST
    };
  }

}
</script>