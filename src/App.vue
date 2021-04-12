<template>
  <div class="app">
    <Header />
    <router-view/>
  </div>
</template>

<script>
import Header from "./components/Header";

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
@import url(assets/css/responsive.css);
@import url(assets/css/reboot.css);

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: white;
  color: white;
}

.app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/*=============================================================
                            LINK
=============================================================*/
.link {
  position: relative;
}

.link::before,
.link::after {
  position: absolute;
  width: 100%;
  height: 1px;
  background-color: white;
  top: 100%;
  left: 0;
}

.link::before {
  content: '';
}

.link--metis {
  text-transform: uppercase;
}

.link--metis::before {
  transform-origin: 100% 50%;
  transform: scale3d(0, 1, 1);
  transition: transform 0.3s;
}

.link--metis:hover::before {
  transform-origin: 0% 50%;
  transform: scale3d(1, 1, 1);
}

</style>