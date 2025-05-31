<template>
    <header id="navBar">
      <h1> Luz do Passado </h1>
      <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/plantas"> Plantas </router-link>
        <router-link to="quiz"> Quiz </router-link>
      </nav>
    </header>
</template>

<script>
  export default {
    name: "navBar"
  }
</script>

<style scoped>
  header {
    background-color: var(--cor01);
    padding: 15px;
    display: flex;
    align-items: center;
    border: 4px solid #263649;
    justify-content: flex-end;
    font-size: 1.5em;
  }

  header h1 {
    font-family: var(--font01);
    color: var(--cor02);
    font-weight: bolder;
    margin: auto;
    margin-left: 0;
  }

  nav a {
    color: var(--cor02);
    margin: 10px;
    text-decoration: none;
    transition: 0.5s;
    justify-self: flex-end;
  }

  nav a:hover {
    color: #d6ad54;
  }
</style>