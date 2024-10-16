<template>
  <div class="beta">
    <div class="container">
      <div class="row">
        <h2 class="heading white">
          We're in beta.<br />
          Get your invite today!
        </h2>
        <router-link class="main-link" to="/"
          >Get an invite
          <img src="https://abdulsamadayoade.github.io/Photosnap/images/arrow-white.svg" alt=""
        /></router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.beta {
  position: relative;
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/bg-beta.jpg);
  background-position: center;
  background-size: cover;
  padding: 50px 0;
}
.beta::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 6px;
  background-image: linear-gradient(to bottom, #5a77ff, #bc7198, #ffc593);
}
.row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
}
h2.heading.white {
  font-size: 3rem;
  line-height: 3.5rem;
  color: white;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 3px;
  width: 50%;
}
@media (max-width: 991px) {
  h2.heading.white {
    font-size: 2.5rem;
    line-height: 3rem;
  }
}
@media (max-width: 768px) {
  .row {
    flex-direction: column;
    align-items: start;
    padding-left: 15px;
  }
  h2.heading.white {
    font-size: 2rem;
    line-height: 2.5rem;
    width: auto;
  }
}
</style>
