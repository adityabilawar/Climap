<template>
  <header :class=" { 'scrolled-nav': scrollPosition} ">
    <nav>
      <div class="branding">
        <img src='C:\Users\adity\Documents\GitHub Repositories\climap\src\assets\logo.png' alt="">
      </div>
      <ul v-show="!mobile" class="navigation">
        <li><router-link class="link" :to="{name:'Home'}">Home</router-link></li>
        <li><router-link class="link" :to="{name:'Home'}">About</router-link></li>
        <li><router-link class="link" :to="{name:'Home'}">Download</router-link></li>
        <li><router-link class="link" :to="{name:'Home'}">Contact</router-link></li>
      </ul>
      <div class='icon'>
        <i @click="toggleMobileNav" v-show="mobile" class="far fa-bars" :class="{'icon-active' : mobileNav}"></i>
      </div>
      <transition name="mobile-nav"></transition>
      https://www.youtube.com/watch?v=u2AwJAFeaKc    8:45
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style lang="sass" scoped></style>