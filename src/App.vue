<template>
  <div id="app">
    <navBar />
    <router-view/>
    <footer_ />
  </div>
</template>

<script>
  import navBar from "./components/navBar.vue"
  import footer_ from "./components/footer.vue"

  export default {
    name: "app",
    components: {
      navBar, 
      footer_
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&family=Oldenburg&family=Passion+One:wght@400;700;900&display=swap');

  * {
    padding: 0;
    margin: 0;
    font-family: var(--font01)
  }

  :root {
    --cor02: bisque;
    /* d6ad54*/
    --cor01: #222;
    --font01: "Oldenburg", serif;
    --font02:"Dancing Script", cursive;
    --font03: "Passion One", sans-serif;
  }

  h2 {
      margin-bottom: 30px;
      padding: 5px;
      border-radius: 10px;
      text-align: left;
      color: var(--cor01);
      background-color: rgba(245, 245, 220, 0.795);
    }
</style>