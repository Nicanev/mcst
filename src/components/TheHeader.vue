<template>
  <header class="header">
    <div class="header__container">
      <div class="header__left">
        <img src="@/assets/img/Logo.svg" class="header__logo" />
        <ul class="header__menu">
          <li><a href="#">Продукция</a></li>
          <li><a href="#">Новости</a></li>
          <li><a href="#">Контакты</a></li>
        </ul>
      </div>
      <div class="header__profile">
        <svg viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path
            d="M9 9.375C10.864 9.375 12.375 7.86396 12.375 6C12.375 4.13604 10.864 2.625 9 2.625C7.13604 2.625 5.625 4.13604 5.625 6C5.625 7.86396 7.13604 9.375 9 9.375Z"
            stroke="black"
            stroke-width="1.2"
          />
          <path
            d="M9 9.375C5.686 9.375 3 12.061 3 15.375H15C15 12.061 12.314 9.375 9 9.375Z"
            stroke="black"
            stroke-width="1.2"
            stroke-linejoin="round"
          />
        </svg>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
.header {
  width: 100%;
  background-color: white;
  &__container {
    display: flex;
    justify-content: space-between;
    height: 4.8rem;
  }
  &__left {
    display: flex;
    align-items: center;
    gap: 3rem;
  }
  &__logo {
    width: 8.1rem;
    height: 3rem;
  }
  &__menu {
    display: flex;
    gap: 2.8rem;
    font-size: 1.4rem;
    li {
      position: relative;
    }
    a {
      color: #4d4d4d;
      transition: 0.2s;
    }
    li::before {
      content: "";
      position: absolute;
      bottom: -1.5rem;
      left: 0;
      width: 100%;
      transition: 0.2s;
      height: 0.2rem;
      background-color: black;
      opacity: 0;
    }
    a:hover {
      color: black;
    }
    li:hover::before {
      content: "";
      position: absolute;
      bottom: -1.6rem;
      left: 0;
      width: 100%;
      transition: 0.2s;
      height: 0.2rem;
      background-color: black;
      opacity: 1;
    }
  }
  &__profile {
    display: flex;
    align-items: center;
    cursor: pointer;
    svg {
      width: 1.8rem;
      height: 1.8rem;
    }
  }
}
</style>
