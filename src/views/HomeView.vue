<script setup>
import footerComponent from '@/components/footerComponent.vue'
</script>

<template>
  <main>
    <div class="benifit">
      <div class="info">
        <h1>Create and share your photo stories.</h1>
        <p>
          Photosnap is a platform for photographers and visual storytellers. We make it easy to
          share photos, tell stories and connect with others.
        </p>
        <router-link class="main-link" to="/"
          >Get an invite
          <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
        /></router-link>
      </div>
      <div class="img"></div>
    </div>
    <div class="benifit white">
      <div class="info">
        <h1>Beautiful stories everytime</h1>
        <p>
          We provide design templates to ensure your stories look terrific. Easily add photos, text,
          embed maps and media from other networks. Then share your story with everyone.
        </p>
        <router-link class="main-link" to="/"
          >View the stories

          <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-black.svg" alt=""
        /></router-link>
      </div>
      <div class="img"></div>
    </div>
    <div class="benifit white">
      <div class="info">
        <h1>Designed for everyone</h1>
        <p>
          Photosnap can help you create stories that resonate with your audience. Our tool is
          designed for photographers of all levels, brands, businesses you name it.
        </p>
        <router-link class="main-link" to="/"
          >View the stories
          <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-black.svg" alt=""
        /></router-link>
      </div>
      <div class="img"></div>
    </div>
    <div class="stories">
      <div class="story">
        <div class="info">
          <h3 class="title">The Mountains</h3>
          <p class="artist">by John Appleseed</p>
          <span></span>
          <router-link class="main-link" to="/"
            >read story
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
          /></router-link>
        </div>
      </div>
      <div class="story">
        <div class="info">
          <h3 class="title">Sunset Cityscapes</h3>
          <p class="artist">by Benjsamin Cruz</p>
          <span></span>
          <router-link class="main-link" to="/"
            >read story
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
          /></router-link>
        </div>
      </div>
      <div class="story">
        <div class="info">
          <h3 class="title">18 Days Voyage</h3>
          <p class="artist">by Alexei Borodin</p>
          <span></span>
          <router-link class="main-link" to="/"
            >read story
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
          /></router-link>
        </div>
      </div>
      <div class="story">
        <div class="info">
          <h3 class="title">Architecturals</h3>
          <p class="artist">by Samantha Brooke</p>
          <span></span>
          <router-link class="main-link" to="/"
            >read story
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
          /></router-link>
        </div>
      </div>
    </div>
    <div class="properties">
      <div class="row container">
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/responsive.svg" alt="" />
          </div>
          <h2>100% Responsive</h2>
          <p>
            No matter which the device you’re on, our site is fully responsive and stories look
            beautiful on any screen.
          </p>
        </div>
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/no-limit.svg" alt="" />
          </div>
          <h2>No Photo Upload Limit</h2>
          <p>
            Our tool has no limits on uploads or bandwidth. Freely upload in bulk and share all of
            your stories in one go.
          </p>
        </div>
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/embed.svg" alt="" />
          </div>
          <h2>Available to Embed</h2>
          <p>
            Embed Tweets, Facebook posts, Instagram media, Vimeo or YouTube videos, Google Maps, and
            more.
          </p>
        </div>
      </div>
    </div>

    <footerComponent></footerComponent>
  </main>
</template>

<style>
.benifit {
  display: flex;
}
.benifit:nth-of-type(2) {
  flex-direction: row-reverse;
}
.benifit .info {
  width: 45%;
  background-color: black;
  display: grid;
  padding: 60px;
}
.benifit.white .info,
.benifit.white .info {
  background-color: white;
}
.benifit .info h1 {
  color: white;
  font-size: 3rem;
  line-height: 3.5rem;
  letter-spacing: 2px;
  font-weight: 500;
  text-transform: uppercase;
}
.benifit .info p {
  color: #868686;
  margin: 25px 0;
}
.benifit.white .info h1,
.benifit.white .info h1,
.benifit.white .info .main-link,
.benifit.white .info .main-link {
  color: black;
}
.benifit:first-of-type .img {
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/create-and-share.jpg);
}
.benifit:nth-of-type(2) .img {
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/beautiful-stories.jpg);
}
.benifit:nth-of-type(3) .img {
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/designed-for-everyone.jpg);
}
.benifit .img {
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 550px;
  width: 55%;
}
.benifit.special .img {
  min-height: 450px;
}
.benifit.special .info h1 {
  margin-top: auto;
}
@media (max-width: 991px) {
  .benifit.special .img {
    background-position: left;
  }
  .benifit.special {
    flex-direction: row !important;
  }
}
@media (max-width: 500px) {
  .benifit.special {
    flex-direction: column-reverse !important;
  }
  .benifit.special .img {
    min-height: 350px;
    background-position: center;
  }
}
.stories {
  display: flex;
  flex-wrap: wrap;
}
.story {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.5)),
    url(https://abdulsamadayoade.github.io/Photosnap/images/mountains.jpg);
  width: 25%;
  min-height: 500px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  padding: 30px;
  display: flex;
  cursor: pointer;
  transition: 0.3s;
  position: relative;
}
.story:nth-of-type(2) {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.5)),
    url(https://abdulsamadayoade.github.io/Photosnap/images/cityscapes.jpg);
}
.story:nth-of-type(3) {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.5)),
    url(https://abdulsamadayoade.github.io/Photosnap/images/18-days-voyage.jpg);
}
.story:last-of-type {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.5)),
    url(https://abdulsamadayoade.github.io/Photosnap/images/architecturals.jpg);
}
.story::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 5px;
  background-image: linear-gradient(27deg, #ffc593 0%, #bc7198 49%, #5a77ff 95%);
  opacity: 0;
  transition: 0.3s;
}
.story:hover {
  transform: translateY(-30px);
}
.story:hover::before {
  opacity: 1;
}
@media (max-width: 991px) {
  .story {
    width: 50%;
  }
}
@media (max-width: 500px) {
  .story {
    width: 100%;
  }
}
.story .info {
  margin-top: auto;
  width: 100%;
  color: white;
}
.story h3.title {
  font-weight: 500;
}

.story span {
  display: block;
  margin: 15px 0;
  width: 100%;
  height: 1px;
  background-color: rgba(255, 255, 255, 0.25);
}
.properties {
  padding: 80px 0;
}
.properties .row {
  display: flex;
  gap: 40px;
  text-align: center;
  flex-wrap: wrap;
}

.properties .img {
  height: 75px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.properties h2 {
  margin: 30px 0px 15px;
  font-weight: 600;
}
.properties p {
  color: #868686;
  max-width: 600px;
  margin: auto;
}
@media (min-width: 992px) {
  .properties .property {
    width: calc((100% / 3) - 27px);
  }
}
@media (max-width: 991px) {
  .benifit .info {
    width: 70%;
  }
  .benifit .img {
    width: 30%;
  }
  .benifit .info h1 {
    font-size: 2.5rem;
    line-height: 3rem;
  }
  .properties .row {
    flex-direction: column;
  }
}
@media (max-width: 768px) {
  .benifit {
    flex-direction: column-reverse !important;
  }
  .benifit .info,
  .benifit .img {
    width: 100%;
  }
  .benifit .img {
    min-height: 450px;
  }
  .benifit .info {
    padding: 60px 40px;
  }
  .benifit .info h1 {
    font-size: 2rem;
    line-height: 2.5rem;
  }
}
</style>
