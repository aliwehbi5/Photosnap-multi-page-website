<script setup>
import footerComponent from '@/components/footerComponent.vue'
import betaComponent from '@/components/betaComponent.vue'
</script>
<template>
  <main>
    <div class="benifit special">
      <div class="info">
        <h1>Pricing</h1>
        <p>
          Create a your stories, Photosnap is a platform for photographers and visual storytellers.
          It’s the simple way to create and share your photos.
        </p>
      </div>
      <div class="img"></div>
    </div>
    <div class="plans">
      <div class="container">
        <div class="toggle-switch">
          <span>Monthly </span>
          <div class="toggle" @click="togglePlan"><span></span></div>
          <span>Yearly </span>
        </div>
        <div class="row">
          <div class="plan">
            <h2>Basic</h2>
            <p>
              Includes basic usage of our platform. Recommended for new and aspiring photographers.
            </p>
            <h1 class="price">{{ monthly ? '$19.00' : '$190.00' }}</h1>
            <p>{{ monthly ? 'per month' : 'per year' }}</p>
            <button class="main-btn">Pick Plan</button>
          </div>
          <div class="plan pro">
            <h2>Pro</h2>
            <p>
              More advanced features available. Recommended for photography veterans and
              professionals.
            </p>
            <h1 class="price">{{ monthly ? '$39.00' : '$390.00' }}</h1>
            <p>{{ monthly ? 'per month' : 'per year' }}</p>
            <button class="main-btn">Pick Plan</button>
          </div>
          <div class="plan">
            <h2>Business</h2>
            <p>
              Additional features available such as more detailed metrics. Recommended for business
              owners.
            </p>
            <h1 class="price">{{ monthly ? '$99.00' : '$990.00' }}</h1>
            <p>{{ monthly ? 'per month' : 'per year' }}</p>
            <button class="main-btn">Pick Plan</button>
          </div>
        </div>
      </div>
    </div>
    <div class="table">
      <div class="container">
        <h1>compare</h1>
        <table>
          <thead>
            <tr>
              <th>Features</th>
              <th>Basic</th>
              <th>Pro</th>
              <th>Business</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Unlimited Story Posting</td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Unlimited Photo Upload</td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Embedding Custom Content</td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Customize Metadata</td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Advanced Metrics</td>
              <td></td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Photo Downloads</td>
              <td></td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Search Engine Indexing</td>
              <td></td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
            <tr>
              <td>Custom Analytics</td>
              <td></td>
              <td></td>
              <td>
                <img src="https://abdulsamadayoade.github.io/Photosnap/images/check.svg" alt="" />
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <betaComponent></betaComponent>
    <footerComponent></footerComponent>
  </main>
</template>

<style scoped>
.benifit.special .img {
  background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/pricing-bg.jpg);
}
@media (max-width: 991px) {
  .benifit.special .img {
    background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/pricing-bg-tablet.jpg);
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
    background-image: url(https://abdulsamadayoade.github.io/Photosnap/images/pricing-bg-mobile.jpg);
  }
}
.plans {
  padding: 50px 0;
}
.plans .row {
  display: flex;
  gap: 40px;
}
.plans .toggle-switch {
  padding: 40px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
.plans .toggle {
  position: relative;
  width: 60px;
  height: 30px;
  background-color: #dfdfdf;
  border-radius: 20px;
  cursor: pointer;
}
.plans .toggle span {
  position: absolute;
  width: 25px;
  height: 25px;
  background-color: black;
  border-radius: 50%;
  top: 2.5px;
  left: 2.5px;
  transition: 0.3s;
}
.plans .toggle-switch > span {
  font-size: 1rem;
  font-weight: bold;
}
.plans .toggled {
  left: calc(100% - 2.5px) !important;
  transform: translateX(-100%);
}
.plans .plan {
  background-color: #f5f5f5;
  padding: 40px;
  text-align: center;
}
.plans .plan.pro {
  position: relative;
  background-color: black;
}
@media (min-width: 992px) {
  .plans .plan.pro {
    transform: scaleY(1.2) scaleX(1.1);
  }
  .plans .row {
    margin-top: 50px;
  }
}
.plans .plan.pro::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 5px;
  background-image: linear-gradient(27deg, #ffc593 0%, #bc7198 49%, #5a77ff 95%);
}
.plans .plan h2 {
  font-weight: bold;
  margin-bottom: 15px;
}
.plans .plan p {
  color: #626262;
}
.plans h1.price {
  font-weight: bold;
  margin-top: 30px;
}
.plans .plan.pro h2,
.plans .pro h1.price {
  color: white;
}
.plans button.main-btn {
  width: 100%;
  margin-top: 40px;
}
.plans .pro button.main-btn {
  color: black;
  background-color: white;
}
.table {
  padding: 50px 0;
}
.table h1 {
  text-align: center;
  font-size: 3rem;
  text-transform: uppercase;
  font-weight: bold;
  letter-spacing: 3px;
  margin-bottom: 40px;
}
.table table {
  width: 100%;
}
.table table {
  width: 100%;
  border-collapse: collapse;
}
.table th,
.table td {
  text-transform: uppercase;
  letter-spacing: 2px;
  font-weight: 500;
  padding: 20px;
}
.table td {
  border-bottom: 1px solid #dfdfdf;
}
.table th {
  border-bottom: 1px solid black;
  text-align: left;
}
.table tr td:not(:first-child),
.table th:not(:first-child) {
  text-align: center;
}
@media (max-width: 991px) {
  .plans .row {
    flex-direction: column;
  }
}
@media (min-width: 769px) and (max-width: 991px) {
  .plans .plan {
    padding-right: 50%;
    text-align: start;
  }
}
@media (max-width: 768px) {
  .table h1 {
    font-size: 2.2rem;
  }
  .table th,
  .table td {
    padding: 15px;
    font-size: 0.7rem;
  }
}
</style>

<script>
import { ref } from 'vue'

export default {
  data() {
    return {
      monthly: ref(true) // Set to true for monthly, false for yearly
    }
  },
  methods: {
    togglePlan() {
      this.monthly = !this.monthly
      document.querySelector('.toggle-switch .toggle span').classList.toggle('toggled')
    }
  }
}
</script>
