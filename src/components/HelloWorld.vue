<template>
  <div class="hello">


    <div class="top_parent">


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

    <!--清除浮动-->
    <div class="clear">


    </div>


    <div class="line marginTopBottom"></div>


    <div class="top_parent">

      <div class="top">
        <span>支付金额:</span>
      </div>

    </div>


    <div class="top">


      <span class="money-span">100元</span>
      <span class="money-span">200元</span>
      <span class="money-span">300元</span>
      <span class="money-span">400元</span>
      <span class="money-span">500元</span>
      <span class="money-span">其他金额</span>


    </div>


    <!--清除浮动-->
    <div class="clear">


    </div>


    <div class="top_parent">
      <div class="top">
        <span class="red">说明</span>
      </div>
    </div>


    <div class="top_parent">

      <div class="top simple-color">
        <span>支付金额有可能会上下浮动，</span>
      </div>
      <br>
      <div class="top simple-color">
        <span>如：100元，最后可能会出现：100.08或99.98</span>
      </div>
      <br>
      <div class="top simple-color">
        <span>实际以支付为准，到账情况不影响</span>
      </div>

    </div>


    <!--清除浮动-->
    <div class="clear">


    </div>


<!--    <div class="submit-button" onclick="go">-->
<!--      <span>确定并提交</span>-->

<!--    </div>-->



    <button
      type="button"
      class="submit-button"
      @click="go"
    >
      确定并提交
    </button>



    <p>
      <router-link to="/Login" tag="Login">
        <a href="/Login">Login</a>
      </router-link>

    </p>




  </div>






</template>

<script>
  export default {
    name: 'HelloWorld',
    data() {
      return {
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }


  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }

  span {
    text-align: start;
  }


  .money-span {
    width: 30%;
    display: inline-block;
    background: #ffffff;
    padding: 5px;
    text-align: center;
    color: #666;
    margin-top: 10px;
    border: #999999 solid 1px;
  }


  .top {
    float: left;
  }

  .top_parent {
    padding: 10px;
  }


  .clear {
    clear: both;
  }


  .line {
    background: #ededed;
    height: 10px;

  }


  .marginTopBottom {
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .red {
    color: red;
  }


  .simple-color {

    color: #999999;


  }


  .input {
    border: #000000;
    margin-left: 8px;
    color: #333333;
  }


  .submit-button {
    color: white;
    background: #23b5e2;
    padding: 15px;
    margin: 60px 15px 15px 15px;
    border-radius: 8px;
  }

  input::-webkit-input-placeholder {
    color: #cccccc;
  }

  input::-moz-placeholder { /* Mozilla Firefox 19+ */
    color: #cccccc;
  }

  input:-moz-placeholder { /* Mozilla Firefox 4 to 18 */
    color: #cccccc;
  }

  input:-ms-input-placeholder { /* Internet Explorer 10-11 */
    color: #cccccc;
  }


</style>
