<script setup>
import SwiperCard from './SwiperCard.vue';

</script>

<template>
  <div class="flame">
    <div class="title_bar">
      <div>
        <svg class="red" xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 10 10" fill="none">
          <circle cx="5" cy="5" r="5" fill="#FF5858" />
        </svg>
        <svg class="yellow" xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 10 10" fill="none">
          <circle cx="5" cy="5" r="5" fill="#FFC72C" />
        </svg>
        <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 10 10" fill="none">
          <circle cx="5" cy="5" r="5" fill="#88D95C" />
        </svg>
      </div>
    </div>
    <div class="screen">
      <SwiperCard></SwiperCard>
    </div>
  </div>
</template>

<style scoped>
.flame {
  display: flex;
  overflow: hidden;

  height: 537px;
  flex-direction: column;
  align-items: flex-start;
  aspect-ratio: 403/262;

  border-radius: 16px 0 0 16px;
  border: 1px solid rgba(0, 0, 0, 0.15);
  background: #FFF;
  box-shadow: 0 2px 12.8px 0 rgba(0, 0, 0, 0.05), 0 8px 32px 0 rgba(0, 0, 0, 0.08);
}

.title_bar {
  display: flex;
  height: 40px;
  padding: 0 16px;
  align-items: center;
  flex-shrink: 0;
  align-self: stretch;

  border-bottom: 1px solid rgba(0, 0, 0, 0.15);
}

.title_bar div {
  display: flex;
  align-items: center;
  gap: 8px;

  background: #FFF;
}

.screen {
  flex: 100;
  align-self: stretch;
  background: #f3f3f3;

  display: flex;
  justify-content: center;
  /* 横方向の中央寄せ */
  align-items: center;
}

@media screen and (max-width: 1024px) {
  .title_bar div {
    display: none;
  }

  .flame {
    width: 100%;
    border-radius: 16px;
  }
}
</style>