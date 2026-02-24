<script setup>
import Hero from '@/components/Hero.vue';
import Device from '@/components/Device.vue';
</script>
<template>
  <Hero></Hero>
  <Device></Device>
</template>
<style scoped>
h1 {
  color: #42b983;
  font-size: 2rem;
  margin-bottom: 20px;
}

p {
  font-size: 1.2rem;
  margin-bottom: 10px;
}

ul {
  list-style-type: disc;
  padding-left: 1.5rem;
}

li {
  font-size: 1rem;
  margin-bottom: 0.5rem;
}

img {
  width: 100px;
}
</style>