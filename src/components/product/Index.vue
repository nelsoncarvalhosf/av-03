<template>
  <div id="app" class="container">
    <img class="brand" alt="Vue logo" width="80px" src="@/assets/logo.png">
    <h2 class="text-right">Shopping Cart: {{this.$store.state.products.length}}</h2>
    <b-container class="col-md-3">
      <div><ProductForm /></div>
      <div class>
        <router-link to="products">listagem de produtos</router-link>
      </div>
    </b-container>
  </div>
</template>

<script>
import ProductForm from "./ProductForm";


export default {
  name: "productApp",
  components: {
    ProductForm,
  },
};
</script>

<style>
#app {
  margin-top: 40px;
}
.qtd-produtos-container {
  margin-top: 20px;
}
</style>