<template>
  <header>
    <div class="flame">
      <RouterLink to="/">
        <img src="../assets/logo.svg" alt="logo">
      </RouterLink>
      <div>
        <ul>
          <li>
            <RouterLink to="/about">このサイトについて</RouterLink>
          </li>
          <li><a href="https://forms.gle/ZzfWt1Z9Ex5hUYN57" target="_blank">
              お問い合わせ<img class="out" src="../assets/open_in_new_24dp_222_FILL0_wght400_GRAD0_opsz24.svg">
            </a></li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style scoped>
.flame {
  display: flex;
  width: auto;
  padding: 1rem 2rem;
  justify-content: space-between;
  align-items: center;

  background: #FFF;
}

ul {
  display: flex;
  align-items: center;
  gap: 2rem;
}

li {
  color: var(--main-text);
  text-align: center;
  font-size: 16px;
  font-weight: 500;
  list-style: none;
}

.out {
  width: 16px;
}

a {
  color: var(--main-text);
  text-decoration: none;
}
</style>
