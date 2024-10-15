<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="logo">
          <router-link to="/">
            <img src="https://abdulsamadayoade.github.io/Photosnap/images/logo.svg" alt="" />
          </router-link>
        </div>
        <div class="left-part">
          <ul class="links">
            <li><router-link to="/stories">Stories </router-link></li>
            <li><router-link to="/features">Features </router-link></li>
            <li><router-link to="/pricing">Pricing </router-link></li>
          </ul>
          <button class="main-btn">Get an invite</button>
        </div>
        <div class="toggle-icon"><span></span><span></span></div>
      </div>
    </div>
  </header>

  <RouterView />
</template>

<style>
header {
  background-color: white;
}
header .row,
header .left-part {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
header .row {
  padding: 30px 0;
}
@media (min-width: 769px) {
  header .logo {
    width: calc(100% / 3);
  }
  header .left-part {
    width: calc((100% / 3) * 2);
  }
  header .toggle-icon span {
    display: none;
  }
}
header .left-part {
  gap: 40px;
}
header ul.links {
  display: flex;
  gap: 40px;
}
header ul li a {
  font-weight: bold;
  cursor: pointer;
  font-size: 1rem;
  text-transform: uppercase;
  color: black;
}
button.main-btn {
  display: block;
  background-color: black;
  border: none;
  font-size: 14px;
  color: white;
  text-transform: uppercase;
  letter-spacing: 2px;
  padding: 15px 30px;
  cursor: pointer;
  transition: 0.3s;
}
button.main-btn:hover {
  background-color: var(--color-gray);
  color: black;
}
@media (min-width: 769px) and (max-width: 991px) {
  header ul.links {
    font-size: 14px;
  }
  button.main-btn {
    padding: 12px 16px;
    font-size: 12px;
  }
}
footer {
  background-color: black;
  padding: 50px 0;
}
footer .row {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
}
footer .row .social {
  display: flex;
  gap: 15px;
  margin-top: 100px;
}
footer .row .links {
  color: white;
  display: grid;
  font-size: 16px;
}
footer .row .links li {
  font-weight: 600;
  text-transform: uppercase;
  transition: 0.3s;
}
footer .row .links li:hover {
  color: var(--color-gray);
}
footer .row .left-part {
  display: flex;
  gap: 100px;
}
.main-link {
  color: white;
  display: flex;
  align-items: center;
  gap: 20px;
  text-decoration: none;
  font-weight: 600;
  text-transform: uppercase;
  font-size: 14px;
}
@media (max-width: 768px) {
  header .left-part {
    position: absolute;
    flex-direction: column;
    background-color: white;
    padding: 45px;
    width: 100%;
    left: 0;
    top: 0;
    transition: 0.3s;
    transform: scaleY(0);
    transform-origin: top;
    z-index: 98;
  }
  header .links {
    flex-direction: column;
  }
  header .toggle-icon {
    position: relative;
    z-index: 99;
    cursor: pointer;
  }
  header .toggle-icon span {
    display: block;
    width: 24px;
    height: 2px;
    background-color: black;
    transition: 0.3s;
  }
  header .toggle-icon span:first-of-type {
    margin-bottom: 6px;
  }
  .toggled header .toggle-icon span:first-of-type {
    margin-bottom: 0;
    transform: rotate(50deg);
  }
  .toggled header .toggle-icon span:last-of-type {
    transform: rotate(-50deg) translate(1px, -1px);
  }
  .toggled header .left-part {
    transform: scaleY(1);
  }
  footer .row {
    flex-direction: column;
    align-items: center;
    gap: 50px;
  }
  footer .row .left-part {
    gap: 50px;
    flex-direction: column;
  }
  footer .row .social {
    margin-top: 50px;
  }
  footer .row .links {
    justify-items: center;
  }
}
</style>

<script>
export default {
  mounted() {
    const toggleIcon = document.querySelector('.toggle-icon')
    console.log(toggleIcon)

    toggleIcon.addEventListener('click', () => {
      document.body.classList.toggle('toggled')
    })
  }
}
</script>
