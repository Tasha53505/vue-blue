<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>
<script>
import { RouterLink, RouterView } from 'vue-router'
</script>


<template>
    <nav >
        <RouterLink to="/">Home </RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
      
  <RouterView />
</template>

<style scoped>
nav {
font-size: 20px;
font-family: Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
color: blueviolet;

}


</style>
