<template>
  <br /><br /><br />
  <div class="title bg-dark">
    <h2 class="text-center dflex">
      <lord-icon
        src="https://cdn.lordicon.com/twprnhsj.json"
        trigger="loop"
        delay="1000"
        colors="primary:#1663c7,secondary:#1663c7"
        style="width: 50px; height: 50px"
      >
      </lord-icon>
      WORKS
    </h2>
  </div>
  <br />
  <div class="container text-center" v-if="works.length > 0">
    <div class="row">
      <div class="section-head col-sm-12"></div>
      <div
        data-aos="zoom-in"
        class="col-lg-4 col-sm-12 col-md-6"
        v-for="work in works"
        :key="work.id"
      >
        <figure class="imghvr-hinge-left">
          <img :src="work.img" />
          <figcaption>
            <h3>{{ work.title }}</h3>
            <div class="dflex w-100" style="margin-top: 2rem">
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-html5"></i> {{ work.html }}
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-css3-alt"></i> {{ work.CSS }}
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-js"></i> {{ work.JS ? work.JS : "No" }}
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-bootstrap"></i>
                {{ work.BootStrap ? work.BootStrap : "No" }}
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-vuejs"></i>
                {{ work.Vue ? work.Vue : "No" }}
              </p>
            </div>

            <div
              class="dflex w-100"
              style="margin-top: 2rem; gap: 0.2rem !important"
            >
              <button type="button" class="btn btn-success">
                <i class="fa-solid fa-link"></i> DEMO
                <a
                  :href="work.demo"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button type="button" class="btn btn-success">
                <i class="fa-regular fa-code-branch"></i> REPO
                <a
                  :href="work.repo"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button class="eye">
                <i class="fa-solid fa-eye"></i> {{ work.views }}
              </button>
            </div>
          </figcaption>
        </figure>
      </div>
      <div data-aos="zoom-in" class="col-lg-4 col-sm-12 col-md-6">
        <figure class="imghvr-hinge-left">
          <img
            src="https://transvelo.github.io/freshcart/assets/images/slider-image-1.jpeg"
          />
          <figcaption>
            <h3>LeaderCommerce</h3>
            <div class="dflex w-100" style="margin-top: 2rem">
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-html5"></i> HTML
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-css3-alt"></i> CSS
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-js"></i> JS
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-bootstrap"></i> BootStrap
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-vuejs"></i> Vue
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark medium p-1 dflex"
              >
                Progress <i class="fa-solid fa-spinner fa-spin"></i>
              </p>
            </div>

            <div
              class="dflex w-100"
              style="margin-top: 2rem; gap: 0.2rem !important"
            >
              <button type="button" class="btn btn-success">
                <i class="fa-solid fa-link"></i> DEMO
                <a
                  href="https://leader-commerce.netlify.app/"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button type="button" class="btn btn-success">
                <i class="fa-regular fa-code-branch"></i> REPO
                <a
                  href="https://github.com/ABDALLAHMETWALLY250/leader-commerce"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button class="eye"><i class="fa-solid fa-eye"></i> 10</button>
            </div>
            <p
              style="border-radius: 5px"
              class="bg-light small text-dark p-1 mt-3"
            >
              Progress <i class="fa-solid fa-spinner fa-spin"></i>
            </p>
          </figcaption>
        </figure>
      </div>

      <div class="col-lg-4"></div>
      <div data-aos="zoom-in" class="col-lg-4 col-sm-12 col-md-6">
        <figure class="imghvr-hinge-left">
          <img
            src="https://thumbs.dreamstime.com/b/vector-logo-coding-companies-company-199205353.jpg"
          />
          <figcaption>
            <h3>Leader-Coding</h3>
            <div class="dflex w-100" style="margin-top: 2rem">
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-html5"></i> HTML
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-css3-alt"></i> CSS
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-js"></i> JS
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-bootstrap"></i> BootStrap
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark p-1 dflex"
              >
                <i class="fa-brands fa-vuejs"></i> Vue
              </p>
              <p
                style="border-radius: 5px"
                class="bg-light text-dark medium p-1 dflex"
              >
                Progress <i class="fa-solid fa-spinner fa-spin"></i>
              </p>
            </div>

            <div
              class="dflex w-100"
              style="margin-top: 2rem; gap: 0.2rem !important"
            >
              <button type="button" class="btn btn-success">
                <i class="fa-solid fa-link"></i> DEMO
                <a
                  href="https://leader-coding.netlify.app/"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button type="button" class="btn btn-success">
                <i class="fa-regular fa-code-branch"></i> REPO
                <a
                  href="https://github.com/ABDALLAHMETWALLY250/leader-coding"
                  target="_blank"
                  rel="noopener noreferrer"
                ></a>
              </button>
              <button class="eye"><i class="fa-solid fa-eye"></i> 10</button>
            </div>
            <p
              style="border-radius: 5px"
              class="bg-light small text-dark p-1 mt-3"
            >
              Progress <i class="fa-solid fa-spinner fa-spin"></i>
            </p>
          </figcaption>
        </figure>
      </div>
      <div class="col-lg-4"></div>
    </div>
  </div>
  <div class="container-fluid" v-else>
    <div
      class="row row-cols-1 row-cols-md-2 g-4 text-center"
      data-aos="zoom-in-left"
      data-aos-duration="1500"
      style="width: 100%; margin: auto"
    >
      <div
        data-aos="zoom-in-right"
        data-aos-duration="1500"
        class="col-lg-4 col-sm-12 col-md-6 wow fadeIn"
        v-for="m in 6"
        :key="m"
      >
        <div width="400" class="card" aria-hidden="true">
          <div class="card-body">
            <h5 class="card-title placeholder-glow">
              <span class="placeholder col-6"></span>
            </h5>
            <p class="card-text placeholder-glow">
              <span class="placeholder col-7"></span>
              <span class="placeholder col-4"></span>
              <span class="placeholder col-4"></span>
              <span class="placeholder col-6"></span>
              <span class="placeholder col-8"></span>
            </p>
            <a
              class="btn btn-primary disabled placeholder col-6"
              aria-disabled="true"
            ></a>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="w-100 my-4">
    <div class="buttons container">
      <router-link to="/skills">
        <a class="hvr-bob">
          <button id="btn">
            <i class="fa-solid fa-angles-left fa-shake"></i>
            <i class="fa-solid fa-bolt"></i> Skills
          </button></a
        ></router-link
      >
      <router-link to="/contact">
        <a class="hvr-bob">
          <button id="btn-two">
            <i class="fa-solid fa-message"></i> Contact
            <i class="fa-solid fa-angles-right fa-shake"></i></button></a
      ></router-link>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      works: null,
    };
  },
  mounted() {
    axios
      .get(
        "https://my-json-server.typicode.com/ABDALLAHMETWALLY250/work-dp/works"
      )
      .then((res) => {
        this.works = res.data;
      });
    window.scrollTo(0, 0);
  },
};
</script>

<style lang="scss" scoped>
h2 {
  color: dodgerblue;
  font-size: 35px;
}
h3 {
  color: dodgerblue;
}
.dark-theme h2,
.dark-theme h3 {
  color: #eee;
}

.dflex {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}
figure {
  background-color: transparent;
  width: 100%;
  height: 400px;
  border-radius: 6px;
  border: 3px solid #000;
  box-shadow: 0 10px 20px -5px #111;
  margin-bottom: 8px;
}
.dark-theme figure {
  background-color: transparent;
  width: 100%;
  height: 400px;
  border-radius: 6px;
  border: 3px solid #eee;
  box-shadow: 0 10px 20px -5px gray;
  margin-bottom: 8px;
}

img {
  width: 100% !important;
  height: 100%;
  border-radius: 6px;
}
img:hover {
  scale: 2;
}
i {
  font-size: 20px;
  margin-right: 5px;
}
.medium {
  display: none !important;
}

@media screen and (max-width: 767px) {
  img {
    max-width: 100%;
    height: auto;
  }
  .n {
    width: 100% !important;
  }
  .medium {
    display: none !important;
  }
  .small {
    display: block !important;
  }
}

@media screen and (min-width: 767px) and (max-width: 1023px) {
  .eye {
    margin-top: 8px;
  }
  .small {
    display: none !important;
  }
  .medium {
    display: block !important;
  }
}

@media screen and (min-width: 1024px) {
  .dflex {
    margin-top: 1rem;
  }
}

.buttons {
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 10px;
}
button,
button:focus {
  font-size: 17px;
  padding: 10px 10px;
  border-radius: 0.7rem;
  background-image: linear-gradient(#25d366);
  border: 2px solid rgb(50, 50, 50);
  border-bottom: 5px solid rgb(50, 50, 50);
  box-shadow: 0px 1px 6px 0px #25d366;
  transform: translate(0, -3px);
  transition: 0.2s;
  display: flex !important;
  transition-timing-function: linear;
}
.fa-js,
.fa-html5,
.fa-css3-alt,
.fa-bootstrap {
  font-weight: normal !important;
}
button:active {
  transform: translate(0, 0);
  border-bottom: 2px solid rgb(50, 50, 50);
}
p {
  margin-right: 7px;
}
.n {
  width: 48%;
}

#btn {
  padding: 10px 8px;
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

#btn:hover {
  color: #ffffff;
  transform: scale(1.1);
  outline: 2px solid #0d6efd;
  box-shadow: 4px 5px 17px -4px #0d6efd;
}

#btn::before {
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

#btn:hover::before {
  width: 250%;
}

#btn-two {
  padding: 10px 8px;
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

#btn-two:hover {
  transform: scale(1.1);
  outline: 2px solid #70bdca;
  color: #0d6efd !important;
  background: #fff !important;
}

#btn-two::before {
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

#btn-two:hover::before {
  width: 250%;
}

.buttons {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1em;
}
.buttons {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
