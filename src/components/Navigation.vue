<template>
<div class="menuBar">
  <b-navbar toggleable="lg" type="dark" variant="info" class="navbar-custom fixed-top">
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-navbar-brand id="logo-desktop" :to="{path:'/'}"><img src="../assets/logo.png" alt="">Hvar House</b-navbar-brand>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="mx-auto ">
        <b-nav-item :to="{path:'/'}">Travel Guide</b-nav-item>
        <b-nav-item :to="{path:'/'}">Custom made tours</b-nav-item>
        <b-nav-item :to="{path:'/'}">experiences</b-nav-item>
      </b-navbar-nav>

      <b-navbar-brand :to="{path:'/'}"><img src="../assets/logo.svg" alt=""></b-navbar-brand>



      <b-navbar-nav class="mx-auto">
        <b-nav-item :to="{path:'/'}">exclusive properties</b-nav-item>
        <b-nav-item :to="{path:'/'}">yachts</b-nav-item>
        <b-nav-item :to="{path:'/'}">contact</b-nav-item>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<script>
import router from 'vue-router';
import Index from '../components/Index'

export default new router({
  routes: [{
    path: '/',
    component: Index
  }, ],
  mode: 'history',
});
</script>
