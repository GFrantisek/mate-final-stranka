<template>
  <header class="header">
    <div class="header-content flex justify-between items-center p-6">
      <!-- Navigation Menu on Top Left -->
      <nav class="flex-1 pt-1">
        <ul class="flex space-x-8">
          <li><nuxt-link to="/">Domov</nuxt-link></li>
          <li><nuxt-link to="/products">Produkty</nuxt-link></li>
          <li><nuxt-link to="/about-us">O nás</nuxt-link></li>
          <li><nuxt-link to="/contact">Kontakt</nuxt-link></li>
        </ul>
      </nav>

      <!-- Logo -->
      <div class="flex-1 flex items-center justify-center">
        <img class="logo" src="~/assets/logo1.png" alt="Company Logo" />
      </div>

      <!-- Basket and Profile Picture Top Right -->
      <div class="icons pt-1 flex-1 flex justify-end space-x-2">
        <img class="basket" src="~/assets/shopping-cart.png" alt="Basket Icon" />
        <img class="user" src="~/assets/user.png" alt="User Icon" />
      </div>
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
    background-color: #fff;
    color: #fff;
  }

  .logo {
    height: 100px; /* adjust as needed */
  }

  .basket,
  .user {
    height: 30px; /* adjust as needed */
  }

  .header-content a {
    color: #008296;
    text-decoration: none;
  }


  .icons {
    justify-content: flex-end; /* Align icons to the right */
  }
</style>
