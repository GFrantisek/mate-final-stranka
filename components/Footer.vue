<template>
  <footer class="footer flex justify-between items-center">
    <div class="pt-1">
      <!-- Logo or company name can be placed here -->
    </div>
    <div class="social-icons flex space-x-2">
      <a href="mailto:zova@zova.sk" class="flex items-center space-x-2">
        <img class="email h-8" src="~/assets/email.png" alt="Email Icon" />
        <p>Email: zova@zova.sk</p>
      </a>
      <a href="https://www.facebook.com/zovasro/" class="flex items-center space-x-2">
        <img class="facebook h-8" src="~/assets/facebook.png" alt="Facebook Icon" />
        <p>Facebook</p>
      </a>
      <a href="https://www.instagram.com/zovasro/" class="flex items-center space-x-2">
        <img class="instagram h-8" src="~/assets/instagram.png" alt="Instagram Icon" />
        <p>Instagram</p>
      </a>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  background-color: #008296;
  color: #fff;
  padding: 1rem;
}
</style>
