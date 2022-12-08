<template>
  <div class="product-chart">
    <h1 class="product-chart_title">Shopping Cart</h1>
    <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>QTY</th>
          <th>Price</th>
          <th>Sub total</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Iphone</td>
          <td>1</td>
          <td>5.000.000</td>
          <td>5.000.000</td>
        </tr>
        <tr>
          <td>Samsung Universi 10X mantaps</td>
          <td>1</td>
          <td>5.000.000</td>
          <td>5.000.000</td>
        </tr>
      </tbody>
    </table>
    <hr>
    <div class="product-chart_summary">
        <p class="product-chart_summary_label">Total</p>
        <p class="product-chart_summary_price">15.000.000</p>
    </div>
    <button>
      <img
        :src="require(`assets/img/gg_shopping-cart.svg`)"
        alt=""
        width="34"
        height="34"
      />
      <p>Checkout</p>
    </button>
  </div>
</template>
