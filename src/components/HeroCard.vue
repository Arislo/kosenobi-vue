<script setup>
import { ref } from 'vue';

const cards = ref(["①2×4", "②10÷5", "③8+6", "④7-3"])
const angle = ref([-10, -30, 0, 10])

const colors = ref(["rgb(206, 17, 17)", "rgb(0, 140, 255)", "rgb(10, 184, 111)", "rgb(211, 122, 7)"])
</script>

<template>
  <div v-for="(num, index) in cards" :key="index" class="flame"
    :style="{ transform: `rotate(${angle[index]}deg)`, backgroundColor: colors[index % colors.length] }">
    <h2>{{ num }}</h2>
  </div>
</template>

<style scoped>
div {
  width: 300px;
  height: 300px;
}

.flame {
  max-width: 220px;
  display: flex;
  margin: 1rem;
  padding: 1rem;
  flex-direction: column;
  /* flex-shrink: 0; */
  align-items: flex-start;
  gap: 24px;
  justify-content: center;

  border-radius: 12px;
  /* background: #fff; */
}

h2 {
  color: #fff;
  font-size: 32px;
  font-weight: 500;

  width: 100%;
  text-align: center;
}
</style>