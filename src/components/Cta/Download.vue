<template>
  <div class="download">
    <h2>Premium EQ</h2>
    <p>
      Get expert-level control with a robust equalizer, volume mixer, and spatial audio. Take your listening experience to a whole new level and access all our incredible features!
    </p>
    <p class="download__price"><span>$4</span>/ month</p>
    <div class="download__buttons">
      <Button :text="'iOS Download'" :icon="'apple'" />
      <Button :text="'Android Download'" :icon="'android'"/>
    </div>
  </div>
</template>

<script>
import Button from './Button.vue'

export default {
  components: {
    Button
  }
}
</script>

<style lang="sass" scoped>
.download
  background-color: $col-card-bg
  border-radius: 1rem
  color: $col-white
  margin-top: -1.6rem
  padding: 4.5rem 3.4rem
  min-height: 52.4rem
  width: 100%
  @include media('medium')
    position: absolute
    top: 15rem
    right: 5.9rem
    padding: 4.7rem 4.8rem 3rem
    margin: 0
    height: 54.3rem
    width: 39.7rem
  @include media('large')
    right: 9.5rem
    top: 8.9rem
    padding: 6rem 5.7rem 6rem 5.4rem
    height: 62.5rem
    width: 44.5rem
  & p
    font-size: 1.8rem
    letter-spacing: -0.5px
    line-height: 2.7rem
    @include media('medium')
      letter-spacing: -0.1px
      line-height: 2.8rem
    @include media('large')
      font-size: 2rem
      letter-spacing: -0.2px
      line-height: 3.4rem
  &__price
    column-gap: 1.9rem
    display: flex
    margin: 4.4rem 0 0 0.8rem
    @include media('medium')
      margin-top: 4.7rem
    @include media('large')
      margin-left: 0.3rem
    & span
      font-size: 6rem
      font-weight: bold
      margin-top: 0.3rem
  &__buttons
    margin: 4.3rem 0 0 0.6rem
    @include media('medium')
      margin-top: 4.4rem
    @include media('large')
      margin: 5.4rem 0

</style>