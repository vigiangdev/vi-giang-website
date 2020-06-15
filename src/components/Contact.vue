<template>
  <div id="contact">
    <div class="container">
      <h1 class="contact-header">Contact</h1>
      <form
        class="contact-form"
        action="mailto:vigiangdev@gmail.com"
        method="post"
        enctype="text/plain"
      >
        <label for="name">Name</label>
        <input type="text" name="name" />
        <br />
        <label for="message">Message</label>
        <textarea name="message" id="message" rows="6"></textarea>
        <br />
        <button class="btn" type="submit">Submit</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style scoped>
#contact {
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  min-height: 650px;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  width: 100%;
}

.contact-header {
  border-width: 0 0 3px 0;
  border-style: solid;
  border-color: #42b983;
}

.contact-form {
  display: flex;
  flex-direction: column;
}

form {
  display: flex;
  justify-content: center;
  width: 100%;
  font-family: "Montserrat", sans-serif;
}

label {
  padding: 0.5rem 0;
}

input {
  font-size: 1rem;
  padding: 0.5rem;
  border: 1px solid #7e828b;
  border-radius: 0.5rem;
}

textarea {
  border: 1px solid #7e828b;
  border-radius: 0.5rem;
  font-size: 1rem;
  padding: 0.5rem;
  font-family: "Montserrat", sans-serif;
}

textarea:focus {
  outline: none;
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

input:focus {
  outline: none;
}

@media (min-width: 640px) {
  .btn {
    padding: 0.75rem 1.5rem;
    font-size: 0.75rem;
  }
}

@media (min-width: 768px) {
  .btn {
    padding: 1rem 2rem;
    font-size: 1rem;
    letter-spacing: 3px;
  }
}

@media (min-width: 1024px) {
  .container {
    width: 768px;
  }
}

@media (min-width: 1200px) {
}
</style>