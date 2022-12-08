<template>
  <div class="product-card">
    <img
      :src="require(`assets/img/product2.png`)"
      alt=""
      width="376"
      height="253"
    />
    <div class="product-card_label">
      <p>Smartphones</p>
    </div>
    <div class="product-card_content">
      <div class="product-card_content_label">
        <p>IPHONE 9</p>
        <h1>An apple mobile which is nothing like apple.</h1>
      </div>
      <div class="product-card_content_price">
        <h1>Rp.5.000.000</h1>
        <div class="product-card_content_price_discount">
          <p class="product-card_content_price_discount_percent">13%</p>
          <p class="product-card_content_price_discount_prevPrice">
            Rp.6.600.000
          </p>
        </div>
      </div>
      <div class="product-card_content_rating">
        <img
          :src="require(`assets/img/star.svg`)"
          alt=""
          width="17"
          height="16"
        />
        <p>4.76</p>
      </div>
      <button>
        <img
          :src="require(`assets/img/gg_shopping-cart.svg`)"
          alt=""
          width="34"
          height="34"
        />
        <p>Add To Cart</p>
      </button>
    </div>
  </div>
</template>
