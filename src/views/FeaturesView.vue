<script setup>
import footerComponent from '@/components/footerComponent.vue'
import betaComponent from '@/components/betaComponent.vue'
</script>
<template>
  <main>
    <div class="benifit special">
      <div class="info">
        <h1>Features</h1>
        <p>
          We make sure all of our features are designed to be loved by every aspiring and even
          professional photograpers who wanted to share their stories.
        </p>
      </div>
      <div class="img"></div>
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
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/custom.svg" alt="" />
          </div>
          <h2>Custom Domain</h2>
          <p>
            With Photosnap subscriptions you can host your stories on your own domain. You can also
            remove our branding!
          </p>
        </div>
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/boost.svg" alt="" />
          </div>
          <h2>Boost Your Experience</h2>
          <p>
            Users that viewed your story or gallery can easily get notifed of new and featured
            stories with our built in mailing list.
          </p>
        </div>
        <div class="property">
          <div class="img">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/drag.svg" alt="" />
          </div>
          <h2>Drag & Drop Image</h2>
          <p>
            Easily drag and drop your image and get beautiful shots everytime. No over the top
            tooling to add friction to creating stories.
          </p>
        </div>
      </div>
    </div>
    <betaComponent></betaComponent>
    <footerComponent></footerComponent>
  </main>
</template>

<style scoped>
.benifit.special .img {
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/features-bg.jpg);
}
@media (max-width: 991px) {
  .benifit.special .img {
    background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/features-bg-tablet.jpg);
  }
}
@media (max-width: 500px) {
  .benifit.special .img {
    background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/features-bg-mobile.jpg);
  }
}
</style>
