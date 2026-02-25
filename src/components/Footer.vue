<template>
  <footer class="footer-001">
    <a href="#">
      <!--お好きな画像を指定してください-->
      <img src="../assets/light-logo.svg">
    </a>
    <nav>
      <ul class="footer-001__list">
        <li><a href="/about" class="footer-001__link">このサイトについて</a></li>
        <li><a href="#" class="footer-001__link">お問い合わせ</a></li>
      </ul>
    </nav>
    <p class="footer-001__copyright">@ 2026 Kosenonbi All rights reserved.</p>
  </footer>
</template>

<style scoped>
.footer-001 {
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: 25px 10px 10px;
  background-color: #FDB7B5;
}

.footer-001__logo {
  width: 130px;
  height: 30px;
}

.footer-001__list {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 0 1.5em;
  list-style-type: none;
  margin: 0 0 .5em;
  padding: .5em;
}

.footer-001__link {
  color: #fff;
  font-weight: 600;
  text-decoration: none;
}

.footer-001 img {
  width: 140px;
}

.footer-001__copyright {
  margin: 0;
  color: #ffffff;
  font-weight: 300;
  font-size: .8em;
}
</style>