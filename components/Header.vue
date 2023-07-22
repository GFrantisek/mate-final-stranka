<template>
  <header class="header">
    <div class="header-content flex justify-between items-center p-6">
      <img class="logo pl-24" src="~/assets/logo.png" alt="Company Logo"/>
      <nav>
        <ul class="flex justify-center items-center space-x-12">
          <li><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="/about">About</nuxt-link></li>
          <li><nuxt-link to="/products">Products</nuxt-link></li>
          <li><nuxt-link to="/contact">Contact</nuxt-link></li>
        </ul>
      </nav>
      <img class="basket pr-24 " src="/path-to-basket-icon.png" alt="Basket Icon">
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
.header {
  background-color: #333;
  color: #fff;
}
.logo, .basket {
  height: 30px;  /* adjust as needed */
}
.header-content a {
  color: #fff;
  text-decoration: none;
}
</style>
