<template>
  <section class="moat error">
    <h1>Uh oh.</h1>
    <p>The page you were looking for could not be found.</p>
    
    <nuxt-link to="/"><a class="btn btn--dk">Reload Page</a></nuxt-link>
  </section>
  
</template>

<style lang="sass" scoped>
.error
  text-align: center
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  min-height: 70vh
  // background-color: pink
  p
    margin-bottom: 20px
  h1
    font-family: $ff-sans-bold
    font-size: 4.4rem
    line-height: 1



</style>