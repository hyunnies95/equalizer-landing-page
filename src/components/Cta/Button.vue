<template>
  <button class="btn">
    <img class="btn__icon" :src="require('@/assets/images/icon-' + icon + '.svg')" :alt="icon">
    {{text}}
  </button>
</template>

<script>
export default {
  props: ['icon', 'text']
}
</script>

<style lang="sass" scoped>
.btn
  border-radius: 1.2rem
  display: flex
  align-items: center
  justify-content: center
  font-size: 1.7rem
  font-weight: bold
  transition: $transition background-color
  height: 5.9rem
  width: 100%
  @include media('medium')
    height: 6rem
  &:first-of-type
    background-color: $col-black
    color: $col-white
    margin-bottom: 1.5rem
    @include media('medium')
      margin-bottom: 1.7rem
    &:hover
      background-color: $col-blue
  &:last-of-type
    background-color: $col-white
    &:hover
      background-color: $col-orange
  &__icon
    margin-right: 0.8rem
</style>