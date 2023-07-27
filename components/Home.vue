<template>
  <div>
    <section class="flex justify-around items-start m-auto py-5 bg-white-600 min-h-[80vh]">
      <!--Product 1 div -->
      <div class="w-1/4 flex flex-col items-center justify-end">
        <div class="relative h-96 bg-white w-full" @mouseover="hover1 = true" @mouseleave="hover1 = false">
          <img :class="{'grayscale': hover1}" src="~/assets/produkt_obr2.png" class="object-cover w-full h-full rounded-lg" alt="Product 1">
          <div class="absolute inset-0 bg-gray-500 text-white flex flex-col justify-center items-center rounded-lg transition-opacity duration-300" :class="{'opacity-0': !hover1, 'opacity-100': hover1}">
            <h2 class="mt-0">Product 1</h2>
            <p class="mb-0">Description for Product 1...</p>
          </div>
        </div>
        <div class="w-full py-2 text-center prices rounded-lg mt-2">
          <h2 class="mt-0">Product 1</h2>
          <p class="mb-0">100€</p>
        </div>
      </div>

      <!--Product 2 div -->
      <div class="w-1/4 flex flex-col items-center justify-end">
        <div class="relative h-96 bg-white w-full" @mouseover="hover2 = true" @mouseleave="hover2 = false">
          <img :class="{'grayscale': hover2}" src="~/assets/product-2.png" class="object-cover w-full h-full rounded-lg" alt="Product 2">
          <div class="absolute inset-0 bg-gray-500 text-white flex flex-col justify-center items-center rounded-lg transition-opacity duration-300" :class="{'opacity-0': !hover2, 'opacity-100': hover2}">
            <h2 class="mt-0">Product 2</h2>
            <p class="mb-0">Description for Product 2...</p>
          </div>
        </div>
        <div class="w-full py-2 text-center prices rounded-lg mt-2">
          <h2 class="mt-0">Product 2</h2>
          <p class="mb-0">200€</p>
        </div>
      </div>

      <!--Product 3 div -->
      <div class="w-1/4 flex flex-col items-center justify-end">
        <div class="relative h-96 bg-white w-full" @mouseover="hover3 = true" @mouseleave="hover3 = false">
          <img :class="{'grayscale': hover3}" src="~/assets/product-3.png" class="object-cover w-full h-full rounded-lg" alt="Product 3">
          <div class="absolute inset-0 bg-gray-500 text-white flex flex-col justify-center items-center rounded-lg transition-opacity duration-300" :class="{'opacity-0': !hover3, 'opacity-100': hover3}">
            <h2 class="mt-0">Product 3</h2>
            <p class="mb-0">Description for Product 3...</p>
          </div>
        </div>
        <div class="w-full py-2 text-center prices rounded-lg mt-2">
          <h2 class="mt-0">Product 3</h2>
          <p class="mb-0">300€</p>
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
.grayscale {
  filter: grayscale(100%);
}

  .prices {
    background-color: #008296;
    color: #fff;
  }
.absolute {
  background-color: rgba(0, 0, 0, 0.5);
  transition: all 0.3s ease;
}

.absolute:hover {
  background-color: rgba(0, 0, 0, 0.7);
}
</style>
