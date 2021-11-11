<template>
  <div class="devise">
    <img class="devise__app" src="@/assets/images/illustration-app.png" alt="phone application">
  </div>
</template>

<style lang="sass" scoped>
.devise
  background-color: black
  background-image: url('~@/assets/images/bg-pattern-2.svg')
  background-repeat: no-repeat
  background-position-x: center
  background-size: 27rem
  border-radius: 1rem 1rem 0 0
  text-align: center
  margin-top: 16.1rem
  height: 38rem
  width: 100%
  @include media('medium')
    border-radius: 1rem
    text-align: left
    padding-left: 6.2rem
    margin-top: 24.9rem
    height: 59.8rem
  @include media('large')
    background-position-x: 33.8rem
    background-position-y: -4rem
    background-size: 31rem
    padding-left: 10.1rem
    margin-top: 32.6rem
  &__app
    margin-top: -9.5rem
    height: 42rem
    @include media('medium')
      margin-top: -13.8rem 
      height: 55.5rem
    @include media('large')
      margin-top: -21.5rem
      height: 65rem
</style>