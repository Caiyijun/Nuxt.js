<template>
  <div>
    <h2>News Index Page</h2>
    <p>NewsID:{{ $route.params.newsId }}</p>
    <ul>
      <li><a href="/">HOME</a></li>
      <!--<li><a href="/news/123op">news1</a></li>-->
      <li><a href="/news/123">news1</a></li>
      <li><a href="/news/456ooo">news2</a></li>
      <li><nuxt-link :to="{name:'news-id',params:{id:123,title: 'i am news'}}">这是用动态路由</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
    export default {
        transition: 'test'
    }
</script>

<style scoped>

</style>
