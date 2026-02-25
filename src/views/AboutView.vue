<script setup>
import HeroCardDemo from '@/components/HeroCardDemo.vue';

</script>

<template>
  <div class="about-view">
    <h1>このサイトについて</h1>
    <p>このサイトは、Vue.js を学習するために制作しました。</p>

    <h2>環境</h2>
    <p>Vue3 + Vite + Vue Router</p>
    <p>API: Composition</p>
    <p>制作日: 2026/02/25</p>
    <p>制作日数: 2日</p>
    <p>Vue学習時間: 約2時間</p>
    <p>制作時間: 約7時間</p>

    <h2>制作理由</h2>
    <p>初めて制作したサイトは Astro だったため、SPA である Vue にも触れてみたいと思い制作しました。</p>
    <p>算数のサイトにした理由はSwiper.jsが有効ではないかと考えたからです。</p>
    <p>ほかのフレームワークにも興味があり、その比較も兼ねています。</p>

    <h2>UI関連</h2>
    <p>カードをめくる部分には Swiper.js を使用しています。</p>
    <p>その他のコンポーネントは Figma でレイアウトを作成し、自作しました。</p>
    <p>Home 部分のカードが右から左に流れる UI がお気に入りです。</p>
    <p>Mac を持っていませんが、Mac 風のデザインを意識して作ってみました。（合っているかはわかりませんが…）</p>

    <h2>学べたこと</h2>
    <p>SPA の基本的な仕組みを理解できました。</p>
    <p>コンポーネントの概念は Astro と似ており、スムーズに制作できました。</p>
    <p>JavaScript が書きやすく、開発体験がとても良かったです。</p>
    <p>style が各コンポーネント内に閉じるため、影響範囲を意識しやすい点も学びでした。</p>

    <h2>お問い合わせ</h2>
    <p>Google Form を利用してお問い合わせフォームを作成しました。</p>
    <p>大学のゼミでも使用していたため、今回も導入しています。実際に送信できます。</p>

    <div class="scroll-gallery">
      <div class="card">
        <HeroCardDemo></HeroCardDemo>
        <HeroCardDemo></HeroCardDemo>
        <HeroCardDemo></HeroCardDemo>
        <HeroCardDemo></HeroCardDemo>
      </div>
    </div>

    <p>複雑なカードを作りたいときに役立ちそうです</p>
    <p class="doko">※カードの中に"すうがく"がまぎれこんでいるかも…</p>

  </div>
</template>

<style>
.about-view {
  padding: 20px;
}

h1 {
  color: var(--main-text);
  font-size: 2rem;
  margin-bottom: 20px;
}

p {
  color: var(--main-text);
  font-size: 1.2rem;
  margin-bottom: 10px;
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
.doko{
  font-size: 0.5rem;
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
</style>