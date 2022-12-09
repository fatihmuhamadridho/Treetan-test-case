<template>
  <div class="product-card">
    <img
      class="product-card_thumb"
      :src="thumb"
      alt=""
      width="376"
      height="253"
    />
    <div class="product-card_label">
      <p>{{ category }}</p>
    </div>
    <div class="product-card_content">
      <div class="product-card_content_label">
        <p>{{ title }}</p>
        <h1>{{ description }}</h1>
      </div>
      <div class="product-card_content_price">
        <h1>${{ price }}</h1>
        <div class="product-card_content_price_discount">
          <p class="product-card_content_price_discount_percent">{{ discountPercentage }}%</p>
          <p class="product-card_content_price_discount_prevPrice">
            ${{ price }}
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
        <p>{{ rating }}</p>
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

<script>
export default {
  props: [
    'thumb',
    'category',
    'title',
    'description',
    'price',
    'discountPercentage',
    'rating',
  ]
}
</script>