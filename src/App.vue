<template>
<div class="collapse navbar-collapse" id="navbarNav">
<ul class="navbar-nav">
<li class="nav-item">
  <a class="nav-link active" aria-current="page" href="#">home</a>
</li>
<li class="nav-item">
  <a class="nav-link" href="#">Features</a>
</li>
<li class="nav-item">
  <a class="nav-link" href="#">Pricing</a>
</li>
<li class="nav-item">
  <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
</li>
</ul>
</div>

<router-link to="/" >홈페이지</router-link>
<router-link to="/list" >리스트페이지</router-link>

<div class="mt-4">
<router-view :블로그글="블로그글"></router-view>
</div>

</template>

<script>
import blog from './assets/blog.js';

export default {
  // eslint-disable-next-line
  name: 'App',
  data(){
    return {
      블로그글 : blog,
    }
  },
  components: {
  
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
