<template>
  <section class="contact">
    <div class="contact__container">
      <div class="contact__title">Наши контакты</div>
      <div class="contact__info">
        <div class="contact__items">
          <div class="contact__item">
            <b>Головной офис АО «МЦСТ» (почтовый адрес):</b> 117437, Москва, ул.
            Профсоюзная, д. 108
          </div>
          <div class="contact__item"><b>Телефон:</b> +7-495-363-96-65</div>
          <div class="contact__item">
            <b>Электронная почта:</b> mcst@mcst.ru
          </div>
        </div>
        <div class="contact__map">
          <iframe
            src="https://yandex.ru/map-widget/v1/?um=constructor%3A9fc421bc2381d61f17e12af290d9d5ce18ed0f2c0636509180f74a1108db5449&amp;source=constructor"
            width="446"
            height="434"
            frameborder="0"
          ></iframe>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
.contact {
  margin-top: 8rem;
  b {
    font-weight: bold;
  }
  &__items {
    margin-top: 5rem;
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
  }
  &__item {
    font-size: 1.4rem;
  }
  &__title {
    font-size: 2.4rem;
    font-weight: bold;
  }
  &__info {
    display: flex;
    justify-content: space-between;
  }
}
</style>
