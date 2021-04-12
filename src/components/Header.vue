<template>
  <div class="header">
    <ul>
      <li>
        <router-link to="/" class="link link--metis">Home</router-link>
      </li>
      <li>
        <router-link to="/" class="link link--metis">Watches</router-link>
      </li>
      <li>
        <router-link to="/" class="link link--metis">History</router-link>
      </li>
    </ul>
    <router-link to="/">
      <img src="../assets/media/images/logo.png" alt="Logo Rolex">
    </router-link>
    <ul>
      <p>Are you a member ?</p>
      <li>
        <router-link to="/" class="link link--metis">Login</router-link>
      </li>
      /
      <li>
        <router-link to="/" class="link link--metis">Register</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Header',
  components: {
  }
}
</script>

<style scoped>
.header {
  height: 15vh;
  position: relative;
  padding: 30px 25px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

img {
  height: 15vh;
}

ul {
  display: flex;
  padding: 20px;
}

ul > li {
  margin: 0 10px;
}

ul:nth-child(3) {
  text-transform: uppercase;
}

ul:nth-child(3) .link::before,
.link::after {
  background-color: gold;
}

ul:nth-child(3) a {
  color: gold;
}

ul:nth-child(3) > li {
  margin: 0 5px!important;
}
</style>