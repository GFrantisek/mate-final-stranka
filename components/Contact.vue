<template>
  <div class="background text-style">
    <p>
      Kontaktná adresa<br>
      <br>
      Zova, s.r.o. <br>
      Fiktívna adresa 69 <br>
      999 99 Fiktívnovo <br>
      Slovensko<br>
      <br>
      Spojiť sa s nami viete cez platformy sociálnych sietí
    </p>
    <div class="pt-1 flex-1 flex justify-beginning space-x-2">
      <img class="email" src="~/assets/email.png" alt="Email Icon" />
      <a href="mailto:zova@zova.sk" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="1">Email: zova@zova.sk</a>
    </div>
    <div class="pt-1 flex-1 flex justify-beginning space-x-2">
      <img class="facebook" src="~/assets/facebook.png" alt="Facebook Icon" />
      <a href="https://www.facebook.com/zovasro/" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="1">Facebook: Zova, s.r.o.</a>
    </div>
    <div class="pt-1 flex-1 flex justify-beginning space-x-2">
      <img class="instagram" src="~/assets/instagram.png" alt="Instagram Icon" />
      <a href="https://www.instagram.com/zovasro/" data-component="link" data-source="inlineLink" data-type="externalLink" data-ordinal="2">Instagram: @zovasro</a>
    </div>

  </div>
</template>


<style scoped>
  .background {
    background-color: #008296;
  }

  .text-style {
    padding: 30px;
    color: #fff;
  }

  .email,
  .facebook,
  .instagram {
    height: 30px; /* adjust as needed */
  }

</style>
