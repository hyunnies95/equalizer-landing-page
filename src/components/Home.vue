<template>
  <section class="home">
    <div class="container">
      <header class="header">
        <Logo />
      </header>
      <About />
      <Cta />
      <Footer />
    </div>
  </section>
</template>

<script>
import Logo from './Logo.vue'
import About from './About.vue'
import Cta from './Cta/Cta.vue'
import Footer from './Footer.vue'


export default {
  components: {
    Logo,
    About,
    Cta,
    Footer
  }
}
</script>

<style lang="sass" scoped>
.home
  background-image: url('~@/assets/images/bg-main-mobile.png')
  background-repeat: no-repeat
  background-position-y: -25rem
  overflow: hidden
  @include media('medium')
    background-image: url('~@/assets/images/bg-main-tablet.png')
    background-position-x: right
  @include media('large')
    background-image: url('~@/assets/images/bg-main-desktop.png')
    background-position-x: center
      
.container
  margin: 0 auto
  max-width: 118.8rem
  @include media('medium')
    padding: 0 3.4rem
    position: relative
  &::before
    @include media('medium')
      background-image: url('~@/assets/images/bg-pattern-1.svg')
      background-repeat: no-repeat
      background-size: contain
      content: ''
      position: absolute
      top: -3.3rem
      right: -4.3rem
      height: 40rem
      width: 27rem
      z-index: 0
    @include media('large')
      top: -3.7rem
      right: -16.4rem
      height: 50rem
      width: 31rem

.header
  padding: 0 2.4rem
  @include media('medium')
    padding: 0
</style>