<script setup>
import Button from './Button.vue';
</script>

<template>
  <div>
    <h2>お問い合わせ</h2>
    <p>本サイトに誤りがありましたら、お知らせください。</p>
    <p>お問い合わせには Google フォームを使用しています。</p>
    <Button class="btn" label="ご連絡はこちらから" url="https://forms.gle/ZzfWt1Z9Ex5hUYN57"></Button>
  </div>
</template>

<style scoped>
div {
  padding: 2rem;
  background-color: #96C787;

  display: flex;
  flex-direction: column;
  align-items: center;
}

h2 {
  color: #000;
  text-align: center;

  /* Heading 1 */
  padding-bottom: 2rem;
  font-size: 50px;
  font-weight: 700;
  /* 47.5px */
  letter-spacing: -1.5px;
}

p {
  color: #000;
  text-align: center;

  /* Paragraph */
  font-size: 15px;
  padding-top: 0.2rem;
  /* 21px */
  letter-spacing: -0.075px;
}

.btn {
  margin: 2rem;
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
