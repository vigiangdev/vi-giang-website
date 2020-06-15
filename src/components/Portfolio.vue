<template>
  <div id="portfolio">
    <h1 class="portfolio-header">Portfolio</h1>
    <div class="homies">
      <div class="homies-container">
        <div class="web-image">
          <img src="@/assets/img/imac-homies.jpg" alt="website-rendering" />
        </div>
        <div class="web-content">
          <div class="description">
            <h3>Homies</h3>
            <p>Homies is a simple web app that provide property seekers the power to search the Realtor API for their dream home.</p>
            <p>Users can refine their search by price, number of bedrooms/bathrooms, property size, and other common features.</p>
          </div>
          <div class="technology">
            <h3>Technology</h3>
            <p>Created with VueJS, VueX, and TailwindCSS.</p>
          </div>
          <button class="btn">Launch</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {}
};
</script>

<style scoped>
#portfolio {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 3rem 2rem 3rem 2rem;
  margin: auto;
  min-height: 650px;
}

.homies {
  border: 1px solid #f5f5f5;
  padding: 2rem;
}

.homies h3 {
  font-size: 1.5rem;
}

.homies-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.portfolio-header {
  border-width: 0 0 3px 0;
  border-style: solid;
  border-color: #42b983;
}
img {
  height: 192px;
}

.web-content {
  margin: 2rem;
}

.btn {
  align-self: center;
  padding: 0.5rem 1rem;
  font-size: 0.5rem;
  letter-spacing: 3px;
  color: #f5f5f5;
  background-color: #42b983;
  text-decoration: none;
  text-transform: uppercase;
  cursor: pointer;
  border-radius: 0.5rem;
  border: none;
  transition: all 0.2s ease-in-out;
  animation-name: shiftBtoT;
  animation-duration: 1s;
  animation-delay: 1s;
  animation-fill-mode: backwards;
}

.btn:hover {
  color: #f5f5f5;
  background-color: #42b983;
  transition: all 0.2s ease-in-out;
}

.btn:focus {
  outline: none;
}

@media (min-width: 640px) {
  .homies-container {
    flex-direction: row;
  }

  img {
    height: 256px;
  }

  .btn {
    padding: 0.75rem 1.5rem;
    font-size: 0.75rem;
  }
}

@media (min-width: 768px) {
  img {
    height: 368px;
  }
}

@media (min-width: 1024px) {
  #portfolio {
    width: 928px;
  }
}
</style>