<template>
  <div class="footer">
    <router-link to="/">
      <img src="../assets/media/images/logo.png" alt="Logo Rolex">
    </router-link>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: #006039;
}

img {
  height: 15vh;
}
</style>