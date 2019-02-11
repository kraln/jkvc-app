<template>
  <div
    class="drawer-toggle"
    role="button"
    @click="$emit('toggle')">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
</template>

<style lang="sass" scoped>
.drawer-toggle 
  display: flex
  flex-direction: column
  justify-content: space-around
  height: 40%
  width: 35px
  cursor: pointer


@include mq(med) 
  .drawer-toggle 
    display: none

.drawer-toggle .bar 
  width: 80%
  height: 3px
  background-color: neutrals(7)

</style>
