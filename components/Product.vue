<template>
  <div class="product" @mouseover="hover = true" @mouseleave="hover = false">
    <div class="product-image">
      <img :src="image" alt="">
    </div>
    <div class="product-description" v-if="hover">
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['image', 'description'],
  data() {
    return {
      hover: false,
    }
  },
}
</script>

<style scoped>
.product {
  position: relative;
}

.product-image img {
  width: 100%;
  transition: opacity 0.5s;
}

.product-description {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(0, 0, 0, 0.5);
  color: white;
  transition: opacity 0.5s;
}

.product:hover .product-image img {
  opacity: 0.5;
}
</style>
