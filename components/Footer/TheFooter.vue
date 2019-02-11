<template>
  <footer class="footer">

    <div class="lurk">Very Hello</div>
    
    <div class="lurkMore">Hoy!</div>

    <div class="copyright">
      <span>&copy;{{ new Date().getFullYear() }} JK Ventures &amp; Consulting UG. All Rights Reserved.</span>
    </div>

  
  </footer>
  
</template>


<style lang="sass" scoped>


.lurk, .lurkMore, .copyright
  margin: 5px 0
  padding: 0 15px
  display: flex
  justify-content: center
  
.lurk
  background-color: neutrals(2)
  a
    padding: 0 10px

.lurkMore
  background-color: neutrals(2)
  font-size: remsize(8)
  font-family: $ff-sans-regular

.copyright
  background-color: neutrals(2)
  font-size: remsize(7)
  font-family: $ff-sans-regular
  

.footer
  background: neutrals(2)
  padding-top: 40px
  padding-bottom: 80px
  border-top: 1px solid neutrals(3)
  text-align: center
  @include mq(med)
    padding-bottom: 50px
    
</style>
