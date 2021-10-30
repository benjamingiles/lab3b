<template>
<div>
  <h1>Your Cart</h1>
  <div v-if="!cart.length"><h2>Cart Empty</h2></div>
  <CartList :products="cart" />
</div>
</template>

<script>
import CartList from "../components/CartList.vue"
export default {
  name: 'Cart',
  components: {
    CartList
  },
  data() {
    return {
    }
  },
  computed: {
    cart() {
      return this.$root.$data.cart;
    }
  },
  methods: {
  }
}
</script>
