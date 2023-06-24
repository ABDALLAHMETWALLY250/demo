<template>
  <div
    id="Home"
    class="alert alert-primary text-center font-monospace fw-bolder fs-normal e wow flash"
    data-aos="fade"
    data-aos-duration="1500"
    style="min-width: 100%"
    role="alert"
  >
    <br />
    <br />
    <br />

    <div data-aos="fade" data-aos-duration="1500" class="welcome">
      <span> Welcome </span>
      <VueWriter style="margin-left: 5px" :array="arr1" />
    </div>
  </div>
  <br />
  <br />
  <br />

  <div data-aos="fade" data-aos-duration="1500" class="row text-center">
    <div class="col-lg-6 col-sm-12 col-md-12">
      <h3 class="fw-bold" id="p">
        {{ x != null ? "HI , " + x.toUpperCase() : "HI My Friend" }}
      </h3>
      <br />

      <div class="name">
        <h3>I'M</h3>
        <h2>ABDALLAH MOHAMED</h2>
      </div>

      <br />
      <div class="descrip">
        <h4 class="d">
          I'M A:
          <VueWriter class="writer" style="margin-left: 5px" :array="arr2" />
        </h4>
      </div>
      <br />
      <p class="detail">
        An ambitious front-end developer who aspires to everything new in
        programming, with more than 2 years of experience working on exciting
        projects. always use the most up-to-date technologies available to
        implement the project in the best possible quality with the ability to
        write clean and professional code.
      </p>
    </div>
    <div class="col-lg-6 col-sm-12 col-md-12">
      <lottie-player
        src="https://assets6.lottiefiles.com/packages/lf20_xRmNN8.json"
        background="transparent"
        speed="1"
        class="lottie"
        loop
        autoplay
      ></lottie-player>
      <br /><br /><br />
    </div>
  </div>
  <div class="w-100   my-2">
    <div class="buttons">
      <router-link to="/contact">
        <a class="hvr-bob">
          <button class="button">
            <i class="fa-solid fa-angles-left fa-shake"></i>
            <i class="fa-solid fa-message"></i> Contact
          </button></a
        ></router-link
      >
      <router-link to="/about">
        <a class="hvr-bob">
          <button class="button-two">
            <i class="fa-solid fa-address-card"></i> About
            <i class="fa-solid fa-angles-right fa-shake"></i></button></a
      ></router-link>
    </div>
  </div>
  <br /><br />
</template>

<script>
export default {
  data() {
    return {
      // x: prompt(" Please Enter Full Name "),
      arr1: [" In My Website"],
      arr2: ["FRONT-END", "CODING", "WEB DESINGER", "VUE DEVELOPER"],
    };
  },
  mounted() {
    window.scrollTo(0, 0);
  },
};
</script>

<style lang="scss" scoped>
.dark-theme .alert {
  background: gray;
}
.alert {
  background: lightblue;
}
.welcome {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
}
.dark-theme .writer {
  color: aqua;
}
.writer {
  color: #f44336;
}
.d {
  text-align: left;
  width: 100%;
  display: flex;
}

.dark-theme h2 {
  color: gold !important;
}
h2 {
  color: darkred !important;
}
.dark-theme h3,
.dark-theme .descrip,
.dark-theme .detail {
  color: #eee;
}
@media screen and (max-width: 767px) {
  h2,
  h3,
  .descrip,
  .detail {
    text-align: center;
    padding: 0;
  }
  h2 {
    font-size: 29px;
  }
  h4 {
    font-size: 22px;
  }
  h3 {
    font-size: 30px;
  }
  .d {
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 28px;
  }
  .detail {
    padding-left: 10px;
    padding-right: 10px;
    font-size: 18px;
  }
  .row {
    display: flex;
    flex-direction: column-reverse;
  }
  .lottie {
    height: 50vh;
    width: 100%;
    margin-left: -9px;
  }
  h2,
  h3,
  .descrip,
  .detail {
    text-align: center;
    padding-left: 10px;
    color: #101213;
  }
  .dark-theme .alert {
    color: blue;
  }
}
@media screen and (min-width: 767px) and (max-width: 1023px) {
  .lottie {
    height: 570px;
    width: 100%;
  }
  .dark-theme .alert {
    color: blue;
  }
  h2 {
    font-size: 40px;
  }
  h4 {
    font-size: 30px;
  }
  h3 {
    font-size: 30px;
  }
  .detail {
    font-size: 20px;
  }
  .col {
    flex: 100%;
  }
  h2,
  h3,
  .descrip,
  .detail {
    text-align: left;
    padding-left: 45px;
    color: #101213;
  }
}
@media screen and (min-width: 1024px) {
  .lottie {
    height: 60vh;
    width: 100%;
  }
  h2 {
    font-size: 40px;
    padding: 0 0.5em !important;
  }
  h4 {
    font-size: 30px;
  }
  h3 {
    font-size: 30px;
  }
  .detail {
    font-size: 20px;
  }
  h2,
  h3,
  .descrip,
  .detail {
    text-align: left;
    padding-left: 100px;
    color: #000;
  }
}

.text-shadow-pop-br {
  -webkit-animation: text-shadow-pop-br 0.6s both;
  animation: text-shadow-pop-br 0.6s both;
}

@-webkit-keyframes text-shadow-pop-br {
  0% {
    text-shadow: 0 0 #555555, 0 0 #555555, 0 0 #555555, 0 0 #555555, 0 0 #555555,
      0 0 #555555, 0 0 #555555, 0 0 #555555;
    -webkit-transform: translateX(0) translateY(0);
    transform: translateX(0) translateY(0);
  }
  100% {
    text-shadow: 1px 1px #555555, 2px 2px #555555, 3px 3px #555555,
      4px 4px #555555, 5px 5px #555555, 6px 6px #555555, 7px 7px #555555,
      8px 8px #555555;
    -webkit-transform: translateX(-8px) translateY(-8px);
    transform: translateX(-8px) translateY(-8px);
  }
}
@keyframes text-shadow-pop-br {
  0% {
    text-shadow: 0 0 #555555, 0 0 #555555, 0 0 #555555, 0 0 #555555, 0 0 #555555,
      0 0 #555555, 0 0 #555555, 0 0 #555555;
    -webkit-transform: translateX(0) translateY(0);
    transform: translateX(0) translateY(0);
  }
  100% {
    text-shadow: 1px 1px #555555, 2px 2px #555555, 3px 3px #555555,
      4px 4px #555555, 5px 5px #555555, 6px 6px #555555, 7px 7px #555555,
      8px 8px #555555;
    -webkit-transform: translateX(-8px) translateY(-8px);
    transform: translateX(-8px) translateY(-8px);
  }
}

.button {
  padding: 12px 18px;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: #0d6efd;
  transition: all 1000ms;
  font-size: 14px;
  position: relative;
  overflow: hidden;
  outline: 2px solid #0d6efd;
}

button:hover {
  color: #ffffff;
  transform: scale(1.1);
  outline: 2px solid #0d6efd;
  box-shadow: 4px 5px 17px -4px #0d6efd;
}

button::before {
  content: "";
  position: absolute;
  left: -50px;
  top: 0;
  width: 0;
  height: 100%;
  background-color: #0d6efd;
  transform: skewX(45deg);
  z-index: -1;
  transition: width 1000ms;
}

button:hover::before {
  width: 250%;
}

.button-two {
  padding: 12px 18px;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  letter-spacing: 4px;
  text-transform: uppercase;
  color: #fff;
  transition: all 1000ms;
  font-size: 14px;
  position: relative;
  overflow: hidden;
  outline: 2px solid #0d6efd;
  background: #0d6efd;
}

.button-two:hover {
  transform: scale(1.1);
  outline: 2px solid #70bdca;
  background: #fff !important;
  color: #0d6efd !important;
}

.button-two::before {
  content: "";
  position: absolute;
  left: -50px;
  top: 0;
  width: 0;
  height: 100%;
  background: #fff !important;
  color: #0d6efd !important;
  transform: skewX(45deg);
  z-index: -1;
  transition: width 1000ms;
}

.button-two:hover::before {
  width: 250%;
}

.buttons {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1em;
}
</style>
