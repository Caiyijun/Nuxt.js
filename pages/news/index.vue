<template>
  <div>
    <h2>News Index Page</h2>
    <p>NewsID:{{ $route.params.newsId }}</p>
    <ul>
      <li><a href="/">HOME</a></li>
      <!--<li><a href="/news/123op">news1</a></li>-->
      <li><a href="/news/123">news1</a></li>
      <li><a href="/news/456">news2</a></li>
    </ul>
  </div>
</template>

<script>
    export default {
        name: "index"
    }
</script>

<style scoped>

</style>
