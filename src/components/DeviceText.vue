<script setup>
import Button from './Button.vue';
</script>

<template>
  <div class="container">
    <div>
      <h2>ためしてみよう！</h2>
      <p>どの端末でもご利用いただけます</p>
    </div>
    <Button label="近日公開" link="#"></Button>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  width: 576px;
  padding: 2rem;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  gap: 32px;
}

h2 {
  align-self: stretch;

  color: #000;
  font-size: 2.6rem;
  font-weight: 700;
  line-height: 110%;
  /* 57.2px */
  letter-spacing: -1.04px;
}

p {
  padding-top: 2rem;
  color: rgba(0, 0, 0, 0.55);
  font-size: 1.2rem;
  font-weight: 500;
  letter-spacing: -0.12px;
}

@media screen and (max-width: 1024px) {
  .container {
    width: 100%;
  }
}

@media screen and (max-width: 650px) {
  h2 {
    font-size: 2rem;
  }

  p {
    font-weight: 500;
  }
}
</style>