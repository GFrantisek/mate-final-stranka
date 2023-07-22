<template>
  <div>
    <section class="products">
      <div class="product">
        <div class="image-container" @mouseover="hover1 = true" @mouseleave="hover1 = false">
          <img src="assets/produkt_obr2.png" alt="Product 1">
          <div class="description" v-show="hover1">
            <h2>Product 1</h2>
            <p>Description for Product 1...</p>
          </div>
        </div>
        <div class="product-info">
          <h2>Product 1</h2>
          <p>$100</p>
        </div>
      </div>
      <div class="product">
        <div class="image-container" @mouseover="hover2 = true" @mouseleave="hover2 = false">
          <img src="path-to-image-2.jpg" alt="Product 2">
          <div class="description" v-show="hover2">
            <h2>Product 2</h2>
            <p>Description for Product 2...</p>
          </div>
        </div>
        <div class="product-info">
          <h2>Product 2</h2>
          <p>$200</p>
        </div>
      </div>
      <div class="product">
        <div class="image-container" @mouseover="hover3 = true" @mouseleave="hover3 = false">
          <img src="path-to-image-3.jpg" alt="Product 3">
          <div class="description" v-show="hover3">
            <h2>Product 3</h2>
            <p>Description for Product 3...</p>
          </div>
        </div>
        <div class="product-info">
          <h2>Product 3</h2>
          <p>$300</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Header from './Header.vue'

export default {
  components: {
    Header
  },
  data() {
    return {
      hover1: false,
      hover2: false,
      hover3: false
    }
  }
}
</script>

<style scoped>
.products {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 60vh;
  margin: 0 auto;
  padding: 20px;
}

.product {
  width: 30%;
  position: relative;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.image-container {
  position: relative;
  width: 100%;
  height: 70%; /* adjust as needed */
}

.product img {
  width: 100%;
  height: 100%; /* adjust as needed */
  display: block;
  margin: auto;
  border-radius: 10px;
}

.product-info {
  width: 100%;
  padding: 10px;
  text-align: center;
  background-color: #f9f9f9;
  border-radius: 10px;
}

.description {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 10px;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.image-container:hover .description {
  opacity: 1;
}

.description h2,
.product-info h2 {
  margin-top: 0;
}

.description p,
.product-info p {
  margin-bottom: 0;
}
</style>
