<template>
	<section class="order">
	    <HeaderTop title="订单列表" />
	    <div class="order_no_login">
	      	<img class="order_img" src="./images/person.png">
	      	<h3 class="order_text">登录后查看外卖订单</h3><br/>
	      	<button class="order_but">立即登陆</button>
	    </div>
    </section>
</template>

<script>
	import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
	export default{
		components:{
			HeaderTop
		}
	}
</script>

<style lang="stylus" rel="stylesheet/stylus">
	@import "../../common/stylus/mixins.styl"
	.order
	    width 100%
	    .header
	    	background-color #02a774
		    position fixed
		    z-index 100
		    left 0
		    top 0
		    width 100%
		    height 45px
		    .header_search
		    	position absolute
		    	left 15px
		    	top 50%
		    	transform translateY(-50%)
		    	width 10%
		    	height 50%
		    	.iconsearch
		    		font-size 25px
		    		color #fff
		    .header_title
		    	position absolute
		    	top 50%
		    	left 60%
		    	transform translate(-40%,-50%)
		    	width 50%
		    	color #fff	
		    .header_login
		    	position absolute
		    	right -15px
		    	color #fff
		    	top 50%
		    	transform translate(-50%,-50%)	
		.order_no_login
			padding-top 140px
			width 60%
			margin 0 auto
			text-align center
			>img
		        display block
		        width 100%
		        height 30%
		    >h3
		  	    padding 10px 0
		        font-size 17px
		        color #6a6a6a
		    >button
		        display inline-block
		        background-color #02a774
		        font-size 14px
		        color #fff
		        border 0
		        outline none
		        border-radius 5px
		        padding 10px 20px
</style>