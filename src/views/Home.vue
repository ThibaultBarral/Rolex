<template>
  <div class="home">
    <video src="../assets/media/videos/hub-collection-watches-cover.mp4" type="video/mp4" autoplay="" playsinline="" loop="" preload="auto"></video>
    <div class="text-top">
      <h1>The Rolex World</h1>
      <h2>Sports, the arts and exploration</h2>
    </div>
    <div class="diagonal-box">
    </div>
    <div class="main-content">
      <div class="main-text-top">
        <h1>Rolex Exploration</h1>
        <p>Rolex makes a unique and lasting contribution to global culture, science and exploration.</p>
      </div>
      <div class="content-product">
        <img src="../assets/media/images/oyster-perpetual.png" alt="Oyster Perpetual">
        <div class="content-text">
          <h1>The essence of the Oyster</h1>
          <div class="line"></div>
          <p>Watches in the Oyster Perpetual range are direct descendants of the original Oyster,
            the world’s first waterproof wristwatch, on which Rolex has built its reputation since 1926.
            These watches benefit from all the fundamental features of the Oyster Perpetual collection – excellent
            chronometric precision, a waterproof Oyster case, and self-winding of the movement via a Perpetual rotor.
            Displaying hours, minutes and seconds, made exclusively of  Oystersteel and featuring a sophisticated finish,
            these are chronometer wristwatches in their purest form.</p>
          <a href="" class="button">Discover All</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>

<style scoped>

.home {
  display: flex;
  justify-content: center;
  flex-direction: column;
}

video {
  min-width: 100%;
  min-height: 100%;
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: -1;
}

.text-top h1 {
  text-transform: uppercase;
  letter-spacing: 15px;
  font-size: 2.95rem;
}

.text-top h1, h2 {
  display: flex;
  justify-content: center;
}

.text-top {
  margin-top: -10vh;
  height: 80vh;
  line-height: 2.5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.diagonal-box {
  background-color: white;
  transform: skewY(-4deg);
  height: 20vh;
  width: 100%;
}

.main-content {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100vh;
  color: black;
}

.main-text-top {
  display: flex;
  justify-content: center;
  margin-top: -10vh;
  z-index: 999;
  padding: 30px 0 60px 0;
}

.main-text-top {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.main-text-top h1 {
  padding: 30px 0;
  text-transform: uppercase;
  letter-spacing: 10px;
  font-size: 2.55rem;
}

.main-text-top > p {
  text-transform: capitalize;
}

.content-product {
  display: flex;
  width: 50%;
}

.content-product img {
  width: 50%;
}

.content-text {
  width: 50%;
  padding-left: 20px;
  position: relative;
}

.content-text h1 {
  text-transform: uppercase;
}

.content-text > .line {
  border: 1px solid black;
  width: 30%;
  margin-top: 20px;
}

.content-text > .line {
  position: absolute;
  left: -10%;
}

.content-text p {
  margin: 40px 0 0 20px;
  line-height: 20px;
  width: 70%;
}

.button {
  transform: scale(1);
  transition: all .2s ease-in-out;
  display: inline-block;
  text-transform: uppercase;
  border: 1px solid black;
  cursor:pointer;
  position: absolute;
  bottom: 0;
  left: 10%;
  font-size:1rem;
  padding:10px 25px;
  text-decoration:none;
}

.button:hover {
  transform: scale(.9);
}

</style>
