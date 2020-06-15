<template>
    <div class="navbar">
        <div class="navlinks">
            <span><router-link v-bind:to="{path: '/#about'}">Home</router-link></span>
            <span><router-link v-bind:to="{path: '/#portfolio'}">Portfolio</router-link></span>
            <span><router-link v-bind:to="{path: '/#contact'}">Contact</router-link></span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Navbar',
    data() {
        return {

        }
    }
}
</script>

<style scoped>
.navbar {
    position: fixed;
    display: flex;
    align-items: center;
    width: 100%;
    background-color: #262A34;
    border-bottom: 5px solid #42B983;
    z-index: 100;
}

.navbar .navlinks {
    display: flex;
}

.navbar .navlinks span {
    padding: 1rem 1.5rem;
}

.navbar .navlinks a {
    text-decoration: none;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #f5f5f5;
    text-transform: uppercase;
    transition: all 0.2s ease-out;
}

.navbar .navlinks a:hover {
    color: #42B983;
    transition: all 0.2s ease-out;
}

</style>