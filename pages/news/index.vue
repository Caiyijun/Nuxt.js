<template>
  <div>
    <h2>News Index Page</h2>
    <p>NewsID:{{ $route.params.newsId }}</p>
    <ul>
      <li><a href="/">HOME</a></li>
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
