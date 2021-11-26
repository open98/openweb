<template>
    <div class="container">
        <div class="my-experience">
            <div class="content">
                <div class="circle">
                    <span>2021</span>
                    <span>YEAR</span>
                </div>
                <div class="date">
                    <div class="item">
                        <span>2021</span>
                        <span>7 月<i class="circle-dot"></i></span>
                    </div>
                    <div class="item">
                        <span>2020</span>
                        <span>6 月<i class="circle-dot"></i></span>
                    </div>
					<div class="item">
					    <span>2019</span>
					    <span>6 月<i class="circle-dot"></i></span>
					</div>
					
                </div>
                <div class="experience">
                    <div class="item" style="margin-top:20px;">
                        <div class="title">
                            广州超级共识有限公司
                        </div>
                        <div class="summary">
                            &lt;IT部&gt;
                        </div>
                        <div class="info">
                            
                        </div>
                    </div>
                    <div class="item" style="margin-top:60px;">
                        <div class="title">
                            柏联智云（广州）科技有限公司
                        </div>
                        <div class="summary">
                            &lt;前端部&gt;
                        </div>
                        <div class="info">
                            
                        </div>
                    </div>
					<div class="item" style="margin-top:90px;">
					    <div class="title">
					        广州澳源区块链技术有限公司
					    </div>
					    <div class="summary">
					        &lt;全栈开发&gt;
					    </div>
					    <div class="info">
					        
					    </div>
					</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
  export default {
    name: "MyExperience"
  }
</script>

<style lang="less" scoped>
    .container{
        position: relative;
        width: 100%;
        height: 100%;
        background: url("../../../assets/images/background4.jpg") no-repeat;
        background-size: cover;
        .my-experience{
            width: 100%;
            height: 100%;
            background: rgba(86, 83, 100, .7);
            display: flex;
            justify-content: center;
            align-items: center;
            
        }
    }
	//手机
	@media screen and (max-width: 760px) {
		.content{
		    position: absolute;
		    top: 50%;
		    left: 50%;
		    -webkit-transform: translate(-50%,-50%);
		    -moz-transform: translate(-50%,-50%);
		    -ms-transform: translate(-50%,-50%);
		    -o-transform: translate(-50%,-50%);
		    transform: translate(-50%,-50%);
		    width: 100%;
		    min-height: 500px;
		    .circle{
		        position: absolute;
		        left: 89px;
		        top: 0;
		        width: 93px;
		        height: 93px;
		        border-radius: 50%;
		        font-size: 30px;
		        font-weight: bold;
		        text-align: center;
		        color: #6bc30d;
		        border: 5px solid #d7d8d8;
		        cursor: pointer;
		        display: flex;
		        flex-direction: column;
		        justify-content: center;
		        -webkit-transition: all 0.3s ease;
		        -moz-transition: all 0.3s ease;
		        -ms-transition: all 0.3s ease;
		        -o-transition: all 0.3s ease;
		        transition: all 0.3s ease;
		        span:nth-child(2){
		            font-size: 15px;
		        }
		        &:hover{
		            -webkit-transform: rotateZ(360deg);
		            -moz-transform: rotateZ(360deg);
		            -ms-transform: rotateZ(360deg);
		            -o-transform: rotateZ(360deg);
		            transform: rotateZ(360deg);
		            background: #6bc30d;
		            color: #fff;
		        }
		    }
		    .date{
		        width: 158px;
		        height: 385px;
		        position: absolute;
		        top: 103px;
		        left: -20px;
		        border-right: 8px solid #d7d8d8;
		        .item{
		            margin-top: 50px;
		            width: 100%;
		            height: 100px;
		            display: flex;
		            justify-content: space-around;
		            align-items: center;
		            span{
		                width: 50%;
		                color: @color-experience;
		            }
		            span:nth-child(1){
		                font-size: 12px;
		                text-align: center;
		            }
		            span:nth-child(2){
		                position: relative;
		                font-size: 18px;
		                text-align: left;
		                .circle-dot{
		                    display: block;
		                    position: absolute;
		                    right: -16px;
		                    top: 0;
		                    width: 20px;
		                    height: 20px;
		                    border-radius: 50%;
		                    border: 2px solid #a6db6d;;
		                    background: #fff;
		                    -webkit-transition: all 0.1s ease;
		                    -moz-transition: all 0.1s ease;
		                    -ms-transition: all 0.1s ease;
		                    -o-transition: all 0.1s ease;
		                    transition: all 0.1s ease;
		                    &:hover{
		                        right: -20px;
		                        top: -5px;
		                        width: 18px;
		                        border-width: 8px;
		                    }
		                }
		                &::before{
		                    content: '';
		                    position: absolute;
		                    right: 0;
		                    top: 50%;
		                    -webkit-transform: translateY(-50%);
		                    -moz-transform: translateY(-50%);
		                    -ms-transform: translateY(-50%);
		                    -o-transform: translateY(-50%);
		                    transform: translateY(-50%);
		                    width: 30%;
		                    height: 1px;
		                    background: #6bc30d;
		                }
		            }
		        }
		    }
		    .experience{
		        position: absolute;
		        right: 20px;
				top: 140px;
		        bottom: 0px;
		        width: 50%;
		        height: auto;
		        display: flex;
		        flex-direction: column;
		        justify-content: space-around;
		        cursor: default;
		        .item{
		            .title{
		                font-size: 20px;
		                color: #fff;
		                -webkit-transition: all 0.3s ease;
		                -moz-transition: all 0.3s ease;
		                -ms-transition: all 0.3s ease;
		                -o-transition: all 0.3s ease;
		                transition: all 0.3s ease;
		                &:hover{
		                    color: #6bc30d;
		                }
		            }
		            .summary{
		                color: #8ca870;
		                font-size: 14px;
		                margin: 4px 0;
		            }
		            .info{
		                color: #fff;
		                font-size: 14px;
		            }
		        }
		
		    }
		}
		
	}
	//pc
	@media screen and (min-width: 760px) {
		.content{
		    position: absolute;
		    top: 50%;
		    left: 50%;
		    -webkit-transform: translate(-50%,-50%);
		    -moz-transform: translate(-50%,-50%);
		    -ms-transform: translate(-50%,-50%);
		    -o-transform: translate(-50%,-50%);
		    transform: translate(-50%,-50%);
		    width: 820px;
		    min-height: 468px;
		    .circle{
		        position: absolute;
		        left: 107px;
		        top: 0;
		        width: 93px;
		        height: 93px;
		        border-radius: 50%;
		        font-size: 30px;
		        font-weight: bold;
		        text-align: center;
		        color: #6bc30d;
		        border: 5px solid #d7d8d8;
		        cursor: pointer;
		        display: flex;
		        flex-direction: column;
		        justify-content: center;
		        -webkit-transition: all 0.3s ease;
		        -moz-transition: all 0.3s ease;
		        -ms-transition: all 0.3s ease;
		        -o-transition: all 0.3s ease;
		        transition: all 0.3s ease;
		        span:nth-child(2){
		            font-size: 15px;
		        }
		        &:hover{
		            -webkit-transform: rotateZ(360deg);
		            -moz-transform: rotateZ(360deg);
		            -ms-transform: rotateZ(360deg);
		            -o-transform: rotateZ(360deg);
		            transform: rotateZ(360deg);
		            background: #6bc30d;
		            color: #fff;
		        }
		    }
		    .date{
		        width: 158px;
		        height: 385px;
		        position: absolute;
		        top: 103px;
		        left: 0;
		        border-right: 8px solid #d7d8d8;
		        .item{
		            margin-top: 50px;
		            width: 100%;
		            height: 100px;
		            display: flex;
		            justify-content: space-around;
		            align-items: center;
		            span{
		                width: 50%;
		                color: @color-experience;
		            }
		            span:nth-child(1){
		                font-size: 12px;
		                text-align: center;
		            }
		            span:nth-child(2){
		                position: relative;
		                font-size: 18px;
		                text-align: left;
		                .circle-dot{
		                    display: block;
		                    position: absolute;
		                    right: -16px;
		                    top: 0;
		                    width: 20px;
		                    height: 20px;
		                    border-radius: 50%;
		                    border: 2px solid #a6db6d;;
		                    background: #fff;
		                    -webkit-transition: all 0.1s ease;
		                    -moz-transition: all 0.1s ease;
		                    -ms-transition: all 0.1s ease;
		                    -o-transition: all 0.1s ease;
		                    transition: all 0.1s ease;
		                    &:hover{
		                        right: -20px;
		                        top: -5px;
		                        width: 18px;
		                        border-width: 8px;
		                    }
		                }
		                &::before{
		                    content: '';
		                    position: absolute;
		                    right: 0;
		                    top: 50%;
		                    -webkit-transform: translateY(-50%);
		                    -moz-transform: translateY(-50%);
		                    -ms-transform: translateY(-50%);
		                    -o-transform: translateY(-50%);
		                    transform: translateY(-50%);
		                    width: 30%;
		                    height: 1px;
		                    background: #6bc30d;
		                }
		            }
		        }
		    }
		    .experience{
		        position: absolute;
		        right: 0;
		        bottom: 0px;
		        width: 630px;
		        height: auto;
		        display: flex;
		        flex-direction: column;
		        justify-content: space-around;
		        cursor: default;
		        .item{
		            .title{
		                font-size: 24px;
		                color: #fff;
		                -webkit-transition: all 0.3s ease;
		                -moz-transition: all 0.3s ease;
		                -ms-transition: all 0.3s ease;
		                -o-transition: all 0.3s ease;
		                transition: all 0.3s ease;
		                &:hover{
		                    color: #6bc30d;
		                }
		            }
		            .summary{
		                color: #8ca870;
		                font-size: 14px;
		                margin: 4px 0;
		            }
		            .info{
		                color: #fff;
		                font-size: 14px;
		            }
		        }
		
		    }
		}
		
	}
</style>
