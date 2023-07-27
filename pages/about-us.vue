<template>
  <div>
    <TheHeader />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '~/components/Header.vue'
import TheFooter from '~/components/Footer.vue'

export default {
  components: {
    TheHeader,
    TheFooter
  }
}
</script>

<style>
/* Add global styles here if needed */
</style>
