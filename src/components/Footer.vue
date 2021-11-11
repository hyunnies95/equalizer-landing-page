<template>
  <footer class="footer">
    <Logo />
    <div class="footer__content">
      <p>
        All rights reserved © Equalizer 2021<br>
        Have any problems? Contact us via social media or email us at <b>equalizer@example.com</b>
      </p>
      <ul class="footer__social">
        <li><a href="#"><img src="@/assets/images/icon-facebook.svg" alt="facebook"></a></li>
        <li><a href="#"><img src="@/assets/images/icon-instagram.svg" alt="instagram"></a></li>
        <li><a href="#"><img src="@/assets/images/icon-twitter.svg" alt="twitter"></a></li>
      </ul>
    </div>
  </footer>
</template>

<script>
import Logo from './Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="sass" scoped>
.footer
  padding: 2.4rem 2.4rem 8rem
  @include media('medium')
    padding: 12rem 0 8rem
  @include media('large')
    display: grid
    grid-template-columns: 28.5rem auto
    padding: 20.2rem 0 4rem
  & .logo
    margin-bottom: 2.8rem
    @include media('large')
      margin: 0
  & p
    margin-bottom: 6.1rem
    @include media('medium')
      font-size: 1.8rem
      line-height: 2.7rem
      margin: 0
      max-width: 36rem
    @include media('large')
      font-size: 1.7rem
      max-width: 40rem
  &__content
    @include media('medium')
      display: flex
      align-items: center
      justify-content: space-between
  &__social
    display: flex
    align-items: center
    column-gap: 1.8rem
    @include media('medium')
      column-gap: 2rem
    & li a
      transition: $transition opacity
      &:hover
        opacity: 0.5
</style>