<template>
    <div>
      <h2>News-content</h2>
      <p>NewsId:{{ $route.params.id }}</p>
      <ul>
        <li><a href="/">HOME</a></li>
      </ul>
    </div>
</template>
<!--校验参数-->
<script>
    export default {
        validate({params}){
          return /^\d+$/.test(params.id);
        },
        data(){
            return {
              title:this.$route.params.title,
            }
        },
        head(){
            return{
              title:this.title,
              meta:[
                {hid:'description',name:'news1',content:'this is news page'}
              ]
            }
        }
    }
</script>

<style scoped>

</style>
