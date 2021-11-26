<template>
  <div class="container">
    <div class="skill">
      <div class="content">
        <div class="title" :class="flag ? 'animated bounceInDown' : '' " >
          技能掌握
        </div>
        <ul class="desc" :class="flag ? 'animated flipInX' : '' " >
          <li>1、掌握HTML5、CSS3、Javascript、JQuery、Bootstrap等主流WEB前端技术</li>
          <li>2、熟练使用Vue全家桶，能够独立将可复用代码封装成组件</li>
          <li>3、熟悉掌握微信小程序、公众号开发</li>
          <li>4、熟练使用less、ES6语法进行开发，对前端工程化、模块化、组件化等有一定理解</li>
          <li>5、熟悉php+Mysql的使用，熟练掌握thinkphp、laravel开源框架的配置和使用</li>
          <li>6、熟练使用Git版本控制工具</li>
		  <li>7、熟练运用Photoshop，office相关软件、大学英语B级、会普通话、粤语</li>
          <li>8、有极强的抗压能力，富有团队精神，有较强的自我驱动力，爱总结、爱分享</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Skill",
    data(){
      return {
        flag: false
      }
    },
    props: {
      curIndex: {
        type: Number,
        default: 1
      }
    },
    watch: {
      curIndex(newVal){
        if(newVal === 3){
          this.flag = true
        }
      }
    }
  }
</script>

<style lang="less" scoped>
  .container{
    width: 100%;
    height: 100%;
    background: url("../../../assets/images/background3.jpg") no-repeat;
    background-size: cover;
    .skill{
      width: 100%;
      height: 100%;
      background: rgba(86, 83, 100, .7);
      display: flex;
      justify-content: center;
      align-items: center;
      
    }
  }
  //手机
  @media screen and (max-width: 768px) {
	  .content{
	    width: 80%;
	    height: 80%;
	    .title{
	      font-size: 30px;
	      text-align: center;
	      margin-bottom: 60px;
	      color: @color-font;
	    }
	    .desc{
	      width: 100%;
	      margin: 0 auto;
	      color: @color-font;
	      font-size: 18px;
	      li{
	        margin-bottom: 10px;
	      }
	    }
	  }
	  
  }
  //pc
  @media screen and (min-width: 768px) {
	  .content{
	    width: 80%;
	    height: 80%;
	    .title{
	      font-size: @font-size-title;
	      text-align: center;
	      margin-bottom: 60px;
	      color: @color-font;
	    }
	    .desc{
	      width: 810px;
	      margin: 0 auto;
	      color: @color-font;
	      font-size: 18px;
	      li{
	        margin-bottom: 10px;
	      }
	    }
	  }
  	  
  }
</style>
