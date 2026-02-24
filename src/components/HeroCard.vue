<script setup>
import { ref } from 'vue';

const cards = ref(["01", "02", "03", "04"])
const angle = ref([-10, -30, 0, 10])
</script>

<template>
  <div v-for="(num, index) in cards" :key="index" class="flame" :style="{ transform: `rotate(${angle[index]}deg)` }">
    <p class="sub-title">Part {{ index + 1 }}</p>
    <h2>{{ num }}</h2>
    <div>
      <p class="title">Title</p>
      <hr>
      <span>かたちかたちかたちかたちかたちかたち
        かたちかたちかたちかたちかたちかたち
      </span>
      <span>かたちかたちかたちかたちかたちかたち
        かたちかたちかたちかたちかたちかたち
      </span>
    </div>
  </div>
</template>

<style scoped>
.haba {
  width: auto;
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

  border-radius: 12px;
  /* background: #fff; */
}

.sub-title {
  color: rgba(102, 102, 102, 0.80);
  font-size: 12px;
  font-weight: 400;
}

h2 {
  color: #000;
  font-size: 32px;
  font-weight: 500;
}

.title {
  color: #3C3C43;
  font-size: 18px;
  font-weight: 500;
}

hr {
  width: 200px;
  height: 1px;
}

span {
  display: inline-block;
  color: #666;
  font-size: 14px;
  font-weight: 400;
}
</style>