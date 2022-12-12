<template>
  <footer class="footer">
    <div class="footer__container">
      <div class="footer__left">
        <img src="@/assets/img/icons/footer-logo.svg" class="footer__logo" />
        <div class="footer__copyright">АО «МЦСТ», 2013-2022</div>
      </div>
      <div class="footer__links">
        <a class="footer__link">Контакты</a>
        <a class="footer__link">Политика конфиденциальности</a>
      </div>
    </div>
  </footer>
</template>

<style lang="scss">
.footer {
  margin-top: 5rem;
  background-color: white;
  width: 100%;
  &__links {
    display: flex;
    gap: 2rem;
    font-size: 1.4rem;
    a {
      cursor: pointer;
    }
  }
  &__container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 6.8rem;
  }
  &__left {
    display: flex;
    gap: 3.4rem;
    align-items: center;
  }
  &__logo {
    width: 8rem;
    height: 3rem;
  }
  &__copyright {
    font-size: 1.4rem;
    color: #696969;
  }
}
</style>
