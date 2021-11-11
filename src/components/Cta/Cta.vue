<template>
  <section class="cta">
    <Devise />
    <Download />
  </section>
</template>

<script>
import Devise from '../Cta/Devise.vue'
import Download from '../Cta/Download.vue'

export default {
  components: {
    Devise,
    Download
  }
}
</script>

<style lang="sass" scoped>
.cta
  @include media('medium')
    position: relative
</style>