<script setup>
import HeroCard from './HeroCard.vue';
</script>

<template>
  <div>
    <div>
      <h1>算数を、もっと身近に。</h1>
      <h2>めくるように学べるスライド式カード</h2>
      <button>
        <RouterLink to="/"></RouterLink>
      </button>
    </div>
    <div class="scroll-gallery">
      <div class="card">
        <HeroCard></HeroCard>
        <HeroCard></HeroCard>
        <HeroCard></HeroCard>
        <HeroCard></HeroCard>
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  align-self: stretch;

  color: #444;
  text-align: center;
  font-size: 3.8rem;
  font-weight: 700;
  line-height: 160%;
  /* 70.4px */
  letter-spacing: -1.28px;
}

h2 {
  color: #444;
  text-align: center;
  font-size: 1.5rem;
  font-weight: 700;
  line-height: 110%;
  /* 30.8px */
  letter-spacing: -0.56px;
}

.scroll-gallery {
  width: 100%;
  overflow: hidden;
}

.card {
  display: flex;
  gap: 16px;
  width: max-content;
  animation: scroll-left 70s linear infinite;
}

@keyframes scroll-left {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-50%);
  }
}

.scroll-gallery:hover .card {
  animation-play-state: paused;
}
@media screen and (max-width: 650px){
  h1 {
    font-size: 2rem;
  }
  h2{
    font-size: 1.2rem;
  }
}
</style>