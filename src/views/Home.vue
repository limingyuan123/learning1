<template>
  <div class="home">
    <Navbar class="navbar"></Navbar>
    <LeftMenu class="leafmenu"></LeftMenu>
  </div>
</template>

<script lang="ts" setup>
import LeftMenu from '../components/LeafMenu.vue'
import Navbar from '../components/Navbar.vue'
</script>

<style>
.home{
  /* display: flex; */
}
.leafmenu{
  height: 100%;
  position: absolute;
  top:60px;
  width: 20%;
}
</style>