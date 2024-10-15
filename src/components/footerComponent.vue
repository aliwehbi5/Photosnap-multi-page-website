<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="left-part">
          <div class="logo">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/logo-white.svg" alt="" />
            <ul class="social">
              <li>
                <a href="#"
                  ><img
                    src="https://abdulsamadayoade.github.io/Photosnap/images/white-FB.svg"
                    alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="https://abdulsamadayoade.github.io/Photosnap/images/white-YT.svg"
                    alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="https://abdulsamadayoade.github.io/Photosnap/images/white-Tw.svg"
                    alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="https://abdulsamadayoade.github.io/Photosnap/images/white-Pin.svg"
                    alt=""
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img
                    src="https://abdulsamadayoade.github.io/Photosnap/images/white-Insta.svg"
                    alt=""
                /></a>
              </li>
            </ul>
          </div>
          <ul class="links">
            <li><router-link to="/">Home </router-link></li>
            <li><router-link to="/stories">Stories </router-link></li>
            <li><router-link to="/features">Features </router-link></li>
            <li><router-link to="/pricing">Pricing </router-link></li>
          </ul>
        </div>
        <router-link class="main-link" to="/"
          >Get an invite
          <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
        /></router-link>
      </div>
    </div>
  </footer>
</template>

<style>
footer ul li a {
  color: white;
}
</style>
