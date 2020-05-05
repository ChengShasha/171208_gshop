<template>
	<div class="msite">
		<!--首页头部-->
		<HeaderTop title="昌平区">
			<span class="header_search" slot="left">
				<i class="iconfont iconsearch"></i>
			</span>
			<span class="header_login" slot="right">
				<span class="header_login_text">登录|注册</span>
			</span>
		</HeaderTop>
		<div class="miste-content-wrapper">
      		<div class="miste-content">
				<!--首页导航-->
				<nav class="msite_nav">
					<div class="swiper-container">
			            <div class="swiper-wrapper">
			            	<div class="swiper-slide">
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/1.jpg">
									</div>
									<span>1甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/1.jpg">
									</div>
									<span>2甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/1.jpg">
									</div>
									<span>3甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/1.jpg">
									</div>
									<span>4甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/1.jpg">
									</div>
									<span>5甜品饮品</span>
								</a>
							</div>
							<div class="swiper-slide">
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/2.jpg">
									</div>
									<span>1甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/3.jpg">
									</div>
									<span>2甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/4.jpg">
									</div>
									<span>3甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/5.jpg">
									</div>
									<span>4甜品饮品</span>
								</a>
								<a href="javascript:" class="link_to_food">
									<div class="food_container">
										<img src="./images/nav/6.jpg">
									</div>
									<span>5甜品饮品</span>
								</a>
							</div>
			            </div>
			        	<div class="swiper-pagination"></div><!--分页器。如果放置在swiper-container外面，需要自定义样式。-->    
					</div>
				</nav>	
			</div>
		</div>
		<!--首页附近商家-->
		<div class="msite_shop_list">
			<div class="shop_header">
				<i class="iconfont iconfujinshangjia"></i>
				<span class="shop_header_title">附近商家</span>
			</div>
			<ShopList/>
		</div>	
	</div>
</template>

<script>
	import Swiper from 'swiper'
	import 'swiper/css/swiper.min.css'
	
	import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
	import ShopList from '../../components/ShopList/ShopList.vue'
	
	export default{
		mounted(){
			//创建一个Swiper实例对象，来实现轮播
			new Swiper('.swiper-container',{
				loop:true, //可以循环轮播
				//如果需要分页器
				pagination: {
				    el: '.swiper-pagination',
				},
			})
		},
		components:{
			HeaderTop,
			ShopList
		}
	}
</script>

<style lang="stylus" rel="stylesheet/stylus">
	@import "../../common/stylus/mixins.styl"
	.msite  
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
		.miste-content-wrapper
			position fixed
			top 45px
			bottom 46px
			width 100%
			.msite_nav
				bottom-border-1px(#e4e4e4)
				margin-top 15px
				height 200px
				background #fff
				.swiper-container
					width 100%
					height 100%
					.swiper-wrapper
						width 100%
						height 100%
						.swiper-slide
							display: flex
							justify-content center
							align-items flex-start
							flex-wrap wrap
							.link_to_food
								width 25%
								.food_container
									display block
									width 100%
									text-align center
									padding-bottom 10px
									font-size 0
									img
										display inline-block
										width 50px
										height 50px
								span
									display block
									width 100%
									text-align center
									font-size 13px
									color #666
					.swiper-pagination
						>span.swiper-pagination-bullet-active	
							background #02a774															
		.msite_shop_list
			top-border-1px(#e4e4e4)
			margin-top 275px
			background #fff
			.shop_header
				padding 10px 10px 0
				.shop_icon
					margin-left 5px
					color #999
				.shop_header_title
					color #999
					font_size 14px
					line-height 20px        						
</style>