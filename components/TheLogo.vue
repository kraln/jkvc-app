<template>
  <svg class="logo" 
    xmlns="http://www.w3.org/2000/svg" 
    viewBox="0 0 283 100.7">
    <title>JKVC</title>
    <g>
      <polygon points="243.7,69.2 232.1,69.2 227.4,61.9 227.4,38 231.2,31.9 244.3,31.9 250.1,41.7 265,34.7 255.1,18 219.7,18 209.8,33.3 209.8,66.5 220.6,82.8 255.1,82.8 265,67.9 250.1,59.1 	"/>
      <polygon points="175.2,68.6 165,18 146.3,18 161.6,82.8 188.1,82.8 203.3,18.1 185.3,18.1 	"/>
      <polygon points="139.1,18 119.1,18 100.1,47.7 100.1,18 82.5,18 82.5,82.8 100.1,82.8 100.1,72.1 109.3,58.9 120.3,82.8 139.4,82.8 121.3,44.4 	"/>
      <polygon points="51.2,61.9 46,69 26.9,56.3 18,70.5 36.7,82.8 57,82.8 68.8,66.5 68.8,18 51.2,18 	"/>
    </g>
  </svg>
</template>

<style lang="sass" scoped>
.logo 
  display: flex
  width: 100px
  margin: 0 20px
  fill: $primary
  transition: all 0.5s ease
  &:hover
    opacity: 0.5
  @include mq(med)
    width: 140px
</style>
