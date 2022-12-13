<template>
    <div class="products">
        <h1>Products:</h1>
    </div>

    <ProductsVue/>
</template>

<script>
import ProductsVue from '../components/Products.vue'

export default {
  name: 'Products',
  components: {
    ProductsVue
  }
}
</script>


<style scoped>
</style>