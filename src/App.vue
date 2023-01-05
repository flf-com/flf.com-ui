<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
    <div class="top-nav">
      <ul style="display: inline-flex ;padding: 10px 20px 30px; list-style-type: none;">
        <li> <a href="/"><u>Home</u></a></li>
        <li><a href="/subjects"><u>Sujects</u></a></li>
        <li><a href="/blogs"><u>Blogs</u></a></li>
        <div class="top-nav-search">
          <li><input type="search"></li>
        </div>
        <li style="float: right;"><a href="/login"><u>Login</u></a></li>
      </ul>

    </div>
  
  <RouterView />
</template>

<style>
.top-nav {
  border-width: 2px;
  border-color: black;
}
.top-nav ul li {
  padding-left: 20px;
  display: block;
  margin: 0px;
}
.top-nav ul li:hover {
  background-color: aqua;
  border-radius: 5px;
}
.top-nav-search {
  align-items: center;
}
</style>

