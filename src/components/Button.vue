<script setup>
const props = defineProps({
  label: {
    type: String,
    required: true
  },
  url: {
    type: String,
    required: true
  }
})
</script>

<template>
  <a :href="url">
    <span>{{ label }}</span>
  </a>
</template>

<style scoped>
a {
  display: flex;
  padding: 8px 13px;
  justify-content: center;
  align-items: center;
  gap: 8px;

  border-radius: 12px;
  background: #434343;
  text-decoration: none;
  
}

span {
  color: #FFF;
  text-align: center;
  font-size: 1rem;
  font-weight: 500;
  line-height: 145%;
  /* 26.1px */
  letter-spacing: -0.09px;
}
</style>