<template>
<div class="header-container">
  <header class="the-header">
    <TheSideNavToggle @toggle="$emit('sidenavToggle')" />

    <div class="logo">
      <nuxt-link to="/">
        <TheLogo />
      </nuxt-link>
    </div>
    
    <div class="spacer"></div>
    <div class="navigation-items">
      <ul class="nav-list">
        <li class="nav-item"><a href="#startup">STARTUP MENTORSHIP</a></li>
        <li class="nav-item"><a href="#iot">IoT DEVELOPMENT</a></li>
        <li class="nav-item"><a href="#speaking">SPEAKING ENGAGEMENTS</a></li>
        <li class="nav-item"><a href="#services">SERVICES</a></li>
        <li class="nav-item"><a href="#contact">CONTACT</a></li>

      </ul>
    </div>
    <!-- <div class="navigation-items">
      <ul class="nav-list">
        <li id="startup" class="nav-item"><nuxt-link to="/">STARTUP MENTORSHIP</nuxt-link></li>
        <li id="iot" class="nav-item"><nuxt-link to="/">IoT DEVELOPMENT</nuxt-link></li>
        <li id="speaking" class="nav-item"><nuxt-link to="/">SPEAKING ENGAGEMENTS</nuxt-link></li>
        <li id="services" class="nav-item"><nuxt-link to="/">SERVICES</nuxt-link></li>
        <li id="contact" class="nav-item"><nuxt-link to="/">CONTACT</nuxt-link></li>
      </ul>
    </div>     -->

  </header>
</div>
</template>

<script>
import TheSideNavToggle from "@/components/Navigation/TheSideNavToggle";
import TheLogo from "@/components/TheLogo";

export default {
  name: "TheHeader",
  components: {
    TheSideNavToggle,
    TheLogo
  }
};
</script>


<style lang="sass" scoped>
.header-container 
  height: 60px


.the-header 
  display: flex
  width: 100%
  position: fixed
  height: 54px
  justify-content: space-around
  align-items: center
  background-color: #eef0f7
  // background-image: linear-gradient(to bottom, rgba(238,240,247,1) 80%, rgba(255,255,255,0) 100%)
  opacity: 1
  z-index: 100
  box-sizing: border-box
  padding: 0 20px


// .logo:hover {
//     fill: pink;
//     }

// .logo {
//   margin: 0 10px;
//   font-size: 1.3rem;
// }

// .logo a {
//   text-decoration: none;
//   color: neutrals(4);
// }

.spacer 
  flex: 1


.navigation-items 
  display: none


// @media (min-width: 768px)
@include mq(med) 
  .navigation-items 
    display: block
  


.nav-list 
  list-style: none
  padding: 0
  margin: 0
  display: flex


.nav-item 
  color: neutrals(7)
  font-family: $ff-sans-regular
  margin: 0 10px
  font-size: remsize(8)


.nav-item a 
  text-decoration: none
  // color: neutrals(2)


.nav-item a:hover,
.nav-item a:active,
.nav-item a.nuxt-link-active 
  // color: $primary

</style>