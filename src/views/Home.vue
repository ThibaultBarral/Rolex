<template>
  <div class="home">
    <video src="../assets/media/videos/hub-collection-watches-cover.mp4" type="video/mp4" autoplay="" playsinline="" loop="" preload="auto"></video>
    <div class="text-top" style="height: 100vh; position: relative">
      <h1>The Rolex World</h1>
      <h2>Sports, the arts and exploration</h2>
      <div class="scroll">
          <p>Scroll</p>
          <i class="fas fa-chevron-down"></i>
      </div>
      <div class="diagonal-box" style="position: absolute; bottom: 0">
    </div>
    </div>
    <div style="height: 5vh"></div>
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
          <a href="#" class="button">Discover All</a>
        </div>
      </div>
      <div class="space"></div>
      <div class="content-product">
        <div class="content-text">
          <h1>Designed For Exploration</h1>
          <div class="line2"></div>
          <p>Presented in 1953, the Explorer is emblematic of the close ties between Rolex and exploration.
            In the 1930s, the brand began to equip numerous Himalayan expeditions with Oyster watches. Among
            these was the group that Sir Edmund Hillary and Tenzing Norgay were part of when they became the
            first to reach the summit of Mount Everest, at 8,848 metres (29,028 feet). This pioneering move
            illustrated the company's ambition to use the world as a laboratory, testing its watches in real
            conditions in order to continually improve them. The feedback that Rolex received from the members
            of these different expeditions therefore had a direct influence on the evolution of its watches,
            making them more precise and robust.</p>
          <a href="#" class="button2">Discover All</a>
        </div>
        <img src="../assets/media/images/explorer.png" alt="Explorer">
      </div>
      <div class="space"></div>
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

.scroll {
  font-weight: bold;
  text-transform: uppercase;
  color: black;
  z-index: 999999;
  position: absolute;
  bottom: 14%;
  right: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  line-height: 25px;
  animation: translate-bottom .3s, bounce 3s ease-in-out infinite;
}

.scroll:hover {
  color: #006039;
  cursor: pointer;

}

@keyframes translate-bottom {
  0% {
    opacity: 0;
    transform: translateY(50px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes bounce {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(16px);
  }
  100% {
    transform: translateY(0);
  }
}

.diagonal-box {
  background-color: white;
  transform: skewY(-4deg);
  height: 20vh;
  width: 100%;
}

.space {
  height: 20vh;
}

.main-content {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
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
  position: absolute;
  left: -10%;
}

.content-text p {
  margin: 40px 0 0 20px;
  line-height: 20px;
  width: 70%;
  text-align: justify;
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

.line2 {
  border: 1px solid black;
  width: 30%;
  margin-top: 20px;
  position: absolute;
  right: -10%;
}

.button2 {
  transform: scale(1);
  transition: all .2s ease-in-out;
  display: inline-block;
  text-transform: uppercase;
  border: 1px solid black;
  cursor:pointer;
  position: absolute;
  bottom: 0;
  right: 10%;
  font-size:1rem;
  padding:10px 25px;
  text-decoration:none;
}

.button2:hover {
  transform: scale(.9);
}
</style>
