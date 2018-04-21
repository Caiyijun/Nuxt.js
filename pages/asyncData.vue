<template>
  <div>
   <p>名字：  {{ info.name }}</p>
   <p>年龄：  {{ info.age }}</p>
   <p>兴趣：  {{ info.interest }}</p>
  </div>
</template>

<script>
  import  axios from 'axios'
  export default {
      data(){
        return{
          name: "蔡奕俊",
          info:''
        }
      },
      // promise方法
    // asyncData(){
    //     return axios.get('https://api.myjson.com/bins/8gdmr')
    //       .then((res)=>{
    //         return {info:res.data}
    //         //为什么不用this，因为这是页面渲染前 的 如果用this的话是没有效果的
    //       })
    // }
    // async方法

    async asyncData(){
        let {data} = await  axios.get('https://api.myjson.com/bins/8gdmr');
        console.log(data);
        return {info:data}
    }
  }
</script>

<style scoped>

</style>
