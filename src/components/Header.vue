<template>
  <header>
    <div class="flame">
      <RouterLink to="/">
        <img src="../assets/logo.svg">
      </RouterLink>
      <div>
        <ul>
          <li>
            <RouterLink to="/info">おしらせ</RouterLink>
          </li>
          <li>
            お問い合わせ
          </li>
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

img {
  width: 20px;
}

ul {
  display: flex;
  align-items: center;
  gap: 2rem;
}

li {
  color: #000;
  text-align: center;
  font-size: 16px;
  font-weight: 500;
  list-style: none;
}

a {
  text-decoration: none;
}
</style>
