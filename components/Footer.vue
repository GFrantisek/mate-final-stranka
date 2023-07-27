<template>
  <footer class="footer">
    <div class="pt-1 flex-1 flex justify-beginning space-x-2">
      <img class="email" src="~/assets/email.png" alt="Email Icon" />
      <a href="mailto:zova@zova.sk" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="1">Email: zova@zova.sk</a>
    </div>
    <div class="pt-1 pb-2 flex-1 flex justify-beginning space-x-2">
      <img class="facebook" src="~/assets/facebook.png" alt="Facebook Icon" />
      <a href="https://www.facebook.com/zovasro/" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="1">Facebook</a>
    </div>
    <div class="pt-1 pb-2 flex-1 flex justify-beginning space-x-2">
      <img class="instagram" src="~/assets/instagram.png" alt="Instagram Icon" />
      <a href="https://www.instagram.com/zovasro/" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="2">Instagram</a>
    </div>
  </footer>
</template>

<style scoped>
  .footer {
    background-color: #008296;
    color: #fff;
    
    text-align: center;
  }

  .email,
  .facebook,
  .instagram {
    height: 30px; /* adjust as needed */
  }
</style>
