<script setup>

</script>
<script>
import { RouterLink, RouterView } from 'vue-router'
</script>


<template>
    <nav >
        <RouterLink to="/">Home </RouterLink>
        <RouterLink to="/about">Gallery</RouterLink>
        <!-- <RouterLink to="/contact">Contact</RouterLink> -->
      </nav>
      
  <RouterView />
</template>

<style scoped>
nav {
font-size: 1.5em;
font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
/* background-color: rgb(126, 206, 243); */
background-color: #1E97BC;
width: 100%;
padding: 0.8em;
}


nav a.router-link-exact-active {
  color: white;
  font-weight: 550;
}

nav a.router-link-exact-active:hover {
  color: rgb(255, 255, 255);
}

nav a {
  display: inline-block;
  padding: 0 1rem;
}

nav a:first-of-type {
  border: 0;
}


</style>
