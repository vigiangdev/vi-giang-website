<template>
  <div id="about">
    <div class="foreground">
      <div class="container">
        <div class="quote quote-1">
          Hello, I'm
          <span>Vi Giang</span>.
        </div>
        <div class="quote quote-2">Web Developer, based in Oakland, CA.</div>
        <router-link v-bind:to="{path: '#portfolio'}">
          <button class="btn">View My Work</button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {};
  }
};
</script>

<style scoped>
#about {
  height: 70vh;
  background-image: url("../assets/img/cover.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  display: flex;
  align-items: center;
  background-color: #f5f5f5;
  background-blend-mode: multiply;
}

.foreground {
  width: 100%;
  height: 100%;
  backdrop-filter: blur(5px);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2.5rem;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-size: 1rem;
}

.container .quote {
  text-align: center;
  padding-bottom: 2rem;
}

.container .quote-1 {
  animation-name: shiftLtoR;
  animation-duration: 1s;
}

.container .quote-2 {
  animation-name: shiftRtoL;
  animation-duration: 1s;
}

.container .quote span {
  color: #42b983;
  font-size: 1.5rem;
}

.btn {
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

@keyframes shiftLtoR {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }
  100% {
    opacity: 1;
    transform: translateX(0px);
  }
}

@keyframes shiftRtoL {
  0% {
    opacity: 0;
    transform: translateX(100px);
  }
  100% {
    opacity: 1;
    transform: translateX(0px);
  }
}

@keyframes shiftBtoT {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0px);
  }
}

@media (min-width: 640px) {
  .foreground {
    padding: 4rem;
  }

  .container {
    font-size: 1.5rem;
  }

  .container .quote {
    padding-bottom: 2.5rem;
  }

  .container .quote span {
    font-size: 2.5rem;
  }
  
  .btn {
    padding: 0.75rem 1.5rem;
    font-size: 0.75rem;
  }
}

@media (min-width: 768px) {
  .foreground {
    padding: 5rem;
  }

  .container {
    font-size: 2rem;
  }

  .container .quote {
    padding-bottom: 3rem;
  }

  .container .quote span {
    font-size: 3rem;
  }

  .btn {
    padding: 1rem 2rem;
    font-size: 1rem;
    letter-spacing: 3px;
  }
}

@media (min-width: 1024px) {
}

@media (min-width: 1200px) {
}
</style>