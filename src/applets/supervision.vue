<template>
    <div>
      <mtitle :titleC="titleC"/>
      <div class="measuring-box">
        <img src="@/assets/img/applets/supervision/01.jpg" alt="">
        <img src="@/assets/img/applets/supervision/02.jpg" alt="">
        <img src="@/assets/img/applets/supervision/03.jpg" alt="">
        <img src="@/assets/img/applets/supervision/04.jpg" alt="">
        <img src="@/assets/img/applets/supervision/05.jpg" alt="">
      </div>
    </div>
</template>

<script>
  export default {
    name: "index",
    components: {
      mtitle: () => import('@/public/TextTitle')
    },
    data(){
      return{
        titleC: {
          type: 'text',
          content: '要监理'
        },
      }
    }
  }
</script>

<style scoped>
  .measuring-box { background: #fff;}
  .drawing { margin-top:30px; padding-bottom: 30px; background:#f7f7f7;}
  .measuring-box h2 { padding: 30px 0 20px 0; font-size: 24px; text-align: center;}
  .measuring-box img { width:100%;}
</style>
