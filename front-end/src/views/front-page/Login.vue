<template>
  <div class="home">
    <div class="blockone" style="margin-bottom: 0.3px">
      <div class="pos">
        <Sign></Sign>
      </div>
    </div>

  </div>
</template>

<script>
// @ is an alias to c
import Sign from '@/components/Sign/sign.vue'
export default {
  name: 'login',
  components: {
    Sign,
  },
  data(){
    return{
      // imagesbox:[{
      //   id:1,
      //   src:'../../assets/login/1.png'
      // },
      //   {
      //     id:2,
      //     src:'../../assets/login/2.png'
      //   }
      // ]

    }
  }
}
</script>
<style scoped>
/*img{*/
/*  width: 100%;*/
/*  height: 100%;*/
/*}*/
  .blockone{
    width: 1519.2px;
    height: 500px;
    background: url("../../assets/login/1.png");
    position: relative;
    left: 0;
    top: 0;
  }
  .pos{
    width: auto;
    height: auto;
    position: absolute;
    right: 100px;
    top: 60px;
    z-index: 60;
  }


</style>