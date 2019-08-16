<template>



  <div class="top_parent">

    <div>3333</div>
    <div>{{count}}</div>
    <div>3333</div>



    <div class="top">
      <span>会员账号</span>
      <input class="input"
             type="text"
             placeholder="请输入您的会员账号"/>
    </div>
    <br>
    <br>

    <div class="top">
      <span>确认账号</span>
      <input class="input" type="text" placeholder="确认您的会员账号"/>
    </div>


  </div>




</template>


<!--count=1314520&money=100-->
<script>
  export default {
    name: 'Login',
    data() {
      return {
        count: this.$route.params.count,
        money: this.$route.params.money,
        msg: '会员账号',
        msg1: '会员账号1'
      }
    },
    mounted() {
    },
    methods: {
      go() {
        this.$router.push({
          path: '/Login',
          query: {
            url: this.link,
            count: '1314520',
            money: '100'
          }
        });
      }
    }


  }


</script>

<style scoped>

</style>
