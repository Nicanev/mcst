<template>
  <section class="product">
    <div class="product__type">
      <div class="product__container">
        <ul class="product__types">
          <li class="product__type-item">
            <img src="@/assets/img/products/elbrus-16c.jpg" />
            <h1>Микропроцессоры и СБИС</h1>
          </li>
          <li class="product__type-item">
            <img
              src="@/assets/img/products/4e8cb-mswtx_448__scheme_top_0256x0240_flat.png"
            />
            <h1>Вычислительные модули</h1>
          </li>
          <li class="product__type-item">
            <img
              src="@/assets/img/products/1e8-2u_tvgi.466256.015__front_above_0256x0128.jpg"
            />
            <h1>Вычислительные машины</h1>
          </li>
        </ul>
      </div>
    </div>
    <div class="product__container">
      <div class="product__title">Продукция</div>
      <ul class="product__products-list">
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
        <li class="product__item">
          <img src="@/assets/img/products/elbrus-16c.jpg" alt="" />
          <h1>Эльбрус 16С</h1>
          <p>
            Сервер высокого уровня в корпусе 2U с 4 процессорами Эльбрус-8СВ.
          </p>
        </li>
      </ul>
    </div>
  </section>
</template>

<style lang="scss">
.product {
  &__title {
    font-size: 2.4rem;
    margin: 2.7rem 0;
    font-weight: bold;
  }
  &__products-list {
    display: flex;
    gap: 2rem;
    flex-wrap: wrap;
  }
  &__item:hover {
    background-color: #8080803a;
  }
  &__item {
    cursor: pointer;
    width: 29rem;
    height: 39.2rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    border: 0.1rem solid #808080;
    img {
      height: 15rem;
      padding-bottom: 2.5rem;
    }
    h1 {
      padding-top: 2.5rem;
      font-size: 2.4rem;
      font-weight: bold;
      border-top: 0.1rem solid #808080;
      margin-bottom: 1rem;
    }
    p {
      font-size: 1.4rem;
      width: 24rem;
    }
  }
  &__type {
    background-color: white;
    padding-top: 2rem;
  }
  &__types {
    display: flex;
    justify-content: center;
    gap: 14rem;
  }
  &__type-item {
    cursor: pointer;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    gap: 0.8rem;
    img {
      height: 8rem;
    }
    h1 {
      max-width: 18rem;
      text-align: center;
      color: #000000;
      font-size: 1.4rem;
      padding-bottom: 2rem;
    }
  }
  &__type-item:hover::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 0.2rem;
    background-color: #000000;
    bottom: 0;
    left: 0;
  }
}
</style>
