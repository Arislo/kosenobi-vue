<script setup>
import DeviceFrame from './DeviceFrame.vue';
import DeviceText from './DeviceText.vue';
</script>

<template>
  <div>
    <DeviceText></DeviceText>
    <DeviceFrame></DeviceFrame>
  </div>
</template>

<style scoped>
div {
  display: flex;
  justify-content: center;
  align-items: center;

  background: #96C787;
}

@media screen and (max-width: 1024px) {
  div{
    display: block;
  }
}
</style>