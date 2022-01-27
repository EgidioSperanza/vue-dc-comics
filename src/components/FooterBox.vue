<template>
    <footer>
        <footer-shop />
        <footer-link />
        <footer-social />
    </footer>
</template>

<script>
import FooterShop from '@/components/FooterShop.vue'
import FooterLink from '@/components/FooterLink.vue'
import FooterSocial from '@/components/FooterSocial.vue'
export default {
      components: { 
      FooterShop,
      FooterLink,
      FooterSocial,
   },

}
</script>

<style lang="scss" scoped>

</style>