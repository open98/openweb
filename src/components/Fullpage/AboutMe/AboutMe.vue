<template>
    <div class="container">
        <div class="about-me">
            <div class="content">
                <div class="title" :class="flag ? 'animated bounceInDown' : '' ">关于我</div>
                <div class="info">
                    <ul class="items" :class="flag ? 'animated bounceInRight' : '' ">
                        <li class="item" >
                            <div class="img-wrapper">
                                <img src="../../../assets/images/i_age.svg" alt="">
                            </div>
                            <p>23岁</p>
                        </li>
                        <li class="item">
                            <div class="img-wrapper">
                                <img src="../../../assets/images/i_edu.svg" alt="">
                            </div>
                            <p>广东科贸职业学院</p>
                        </li>
                        <li class="item">
                            <div class="img-wrapper">
                                <img src="../../../assets/images/i_site.svg" alt="">
                            </div>
                            <p>广东/佛山</p>
                        </li>
                        <li class="item">
                            <div class="img-wrapper">
                                <img src="../../../assets/images/i_status.svg" alt="">
                            </div>
                            <p>寻找机遇</p>
                        </li>
                    </ul>
                </div>
                <div class="desc" :class="flag ? 'animated bounceInLeft' : '' ">
                    <p>
                        我叫区学澎，来自广东佛山，2019年毕业于广东科贸职业学院软件技术专业，毕业后一直从事IT工作。
                    </p>
                    <p>
                        我喜欢敲代码，但这并不能让我满足，相较于其它语言，前端更易于去完成一个完整的项目，于是我开始学习研究前端技术。
                        从最基础的前端三件套CSS、HTML、Javascript到less、ES6、TS，再从Jquery、bootstrap等框架到基于MVVM的Vue框架等。
                        这个过程让我收起了对前端页面仔的呆板印象，取而代之的是一种敬畏的心态。现在前端业务的复杂程度已经不输于后端。
                    </p>
                    
                </div>
                
            </div>
        </div>
    </div>
</template>

<script>
  export default {
    name: "AboutMe",
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
        if(newVal === 2){
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
        background: url("../../../assets/images/background2.jpg") no-repeat;
        background-size: cover;
        .about-me{
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            background: rgba(86, 83, 100, .7);
            
        }
    }
     //手机
     @media screen and (max-width: 768px) {
		 .content{
		     width: 90%;
		     height: 90%;
		     color: @color-font;
		     .title{
		         font-size: 30px;
		         text-align: center;
		         margin-bottom: 30px;
		     }
		     .info{
		         width: 100%;
		         margin: 0 auto;
		         display: flex;
		         justify-content: center;
		         .items{
		             display: flex;
		             flex-direction: row;
		             justify-content: center;
		             align-content: space-between;
		             .item{
		                 width: 100%;
		                 height: auto;
		                 display: flex;
		                 flex-direction: column;
		                 align-items: center;
		                 .img-wrapper{
		                     width: 80px;
		                     height: 80px;
		                     border-radius: 50%;
		                     background: @color-blue;
		                     display: flex;
		                     justify-content: center;
		                     align-items: center;
		                     img{
		                         width: 80px;
		                         height: 80px;
		                     }
		                 }
		             }
		         }
		     }
		     .desc{
		         width: 80%;
		         margin: 20px auto;
		         font-size: 18px;
		         p{
		             margin-bottom: 10px;
		             line-height: 27px;
		         }
		     }
		     .blog-addr{
		         width: 80%;
		         margin: 0 auto;
		         a{
		             font-size: 18px;
		             color: @color-blue;
		             &:nth-child(1){
		                 margin-right: 5px;
		             }
		         }
		 
		     }
		 }
		 
	 }
	 //pc
	 @media screen and (min-width: 768px) {
	 	.content{
	 	    width: 80%;
	 	    height: 80%;
	 	    color: @color-font;
	 	    .title{
	 	        font-size: @font-size-title;
	 	        text-align: center;
	 	        margin-bottom: 60px;
	 	    }
	 	    .info{
	 	        width: 80%;
	 	        margin: 0 auto;
	 	        display: flex;
	 	        justify-content: center;
	 	        .items{
	 	            display: flex;
	 	            flex-direction: row;
	 	            justify-content: center;
	 	            align-content: space-between;
	 	            .item{
	 	                width: 200px;
	 	                height: 155px;
	 	                display: flex;
	 	                flex-direction: column;
	 	                align-items: center;
	 	                .img-wrapper{
	 	                    width: 100px;
	 	                    height: 100px;
	 	                    border-radius: 50%;
	 	                    background: @color-blue;
	 	                    display: flex;
	 	                    justify-content: center;
	 	                    align-items: center;
	 	                    img{
	 	                        width: 80px;
	 	                        height: 80px;
	 	                    }
	 	                }
	 	            }
	 	        }
	 	    }
	 	    .desc{
	 	        width: 80%;
	 	        margin: 40px auto;
	 	        font-size: 18px;
	 	        p{
	 	            margin-bottom: 10px;
	 	            line-height: 27px;
	 	        }
	 	    }
	 	    .blog-addr{
	 	        width: 80%;
	 	        margin: 0 auto;
	 	        a{
	 	            font-size: 18px;
	 	            color: @color-blue;
	 	            &:nth-child(1){
	 	                margin-right: 5px;
	 	            }
	 	        }
	 	
	 	    }
	 	}	 
	 }
</style>
