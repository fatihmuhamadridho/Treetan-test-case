<template>
  <div class="homepage">
    <div class="homepage_card">
      <ProductCard
        v-for="product in products.products"
        :key="product.id"
        :thumb="product.images[0]"
        :category="product.category"
        :title="product.title"
        :description="product.description"
        :price="(product.price)"
        :discountPercentage="product.discountPercentage"
        :rating="product.rating"
      />
    </div>
    <div class="homepage_cart">
      <ProductChart :chart="chart" />
    </div>
  </div>
</template>

<script>
import "./home.module.scss";
const chart = {
  summary: 123123
}

export default {
  head: {
    title: "TREETAN TEST CASE",
  },
  data: () => ({
    products: null,
    chart: chart
  }),
  async fetch() {
    this.products = await fetch("https://dummyjson.com/products").then((res) =>
      res.json()
    );
  },
};
// async function test() {
//   console.log("Test");
// }
// test();
// export default {
//   data: () => ({
//     products: []
//   }),
//   async fetch() {
//     this.products = await fetch('https://dummyjson.com/products').then(res => console.log(res.json()))
//   }
// }
</script>
