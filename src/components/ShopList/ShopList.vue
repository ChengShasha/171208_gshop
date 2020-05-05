<template>
		<div class="shop_container">
				<ul class="shop_list">
					<li class="shop_li border-1px">
						<a>
							<div class="shop_left">
								<img class="shop_img" src="./images/shop/1.jpg">
							</div>
							<div class="shop_right">			
								<section class="shop_detail_header">
					            	<h4 class="shop_title ellipsis">锄禾日当午</h4>
					            </section>
					            <section class="shop_rating_order">
					              	<section class="shop_rating_order_left">
						              	<div>
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              	</div>					            
						                <div class="rating_section">4.8</div>
						                <div class="order_section">月售107单</div>
					              	</section>
						            <section class="shop_rating_order_right">
						                <span class="delivery_style delivery_right">美团专送</span>
						            </section>
					            </section>
					            <section class="shop_distance">
					              <p class="shop_delivery_msg">
					                <span>￥20起送/配送费约¥5</span>					          
					              </p>
					            </section>
							</div>
						</a>
					</li>
					<li class="shop_li border-1px">
						<a>
							<div class="shop_left">
								<img class="shop_img" src="./images/shop/1.jpg">
							</div>
							<div class="shop_right">			
								<section class="shop_detail_header">
					            	<h4 class="shop_title ellipsis">锄禾日当午</h4>
					            </section>
					            <section class="shop_rating_order">
					              	<section class="shop_rating_order_left">
						              	<div>
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              	</div>					            
						                <div class="rating_section">4.8</div>
						                <div class="order_section">月售107单</div>
					              	</section>
						            <section class="shop_rating_order_right">
						                <span class="delivery_style delivery_right">美团专送</span>
						            </section>
					            </section>
					            <section class="shop_distance">
					              <p class="shop_delivery_msg">
					                <span>￥20起送/配送费约¥5</span>					          
					              </p>
					            </section>
							</div>
						</a>
					</li>
					<li class="shop_li border-1px">
						<a>
							<div class="shop_left">
								<img class="shop_img" src="./images/shop/1.jpg">
							</div>
							<div class="shop_right">			
								<section class="shop_detail_header">
					            	<h4 class="shop_title ellipsis">锄禾日当午</h4>
					            </section>
					            <section class="shop_rating_order">
					              	<section class="shop_rating_order_left">
						              	<div>
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              		<a href="images/stars/star24_on@2x.png" />
						              	</div>					            
						                <div class="rating_section">4.8</div>
						                <div class="order_section">月售107单</div>
					              	</section>
						            <section class="shop_rating_order_right">
						                <span class="delivery_style delivery_right">美团专送</span>
						            </section>
					            </section>
					            <section class="shop_distance">
					              <p class="shop_delivery_msg">
					                <span>￥20起送/配送费约¥5</span>					          
					              </p>
					            </section>
							</div>
						</a>
					</li>
				</ul>
			</div>
		
</template>

<script>
</script>

<style lang="stylus" rel="stylesheet/stylus">
	@import "../../common/stylus/mixins.styl"
	.shop_container
				margin_bottom 50px
				.shop_list
					.shop_li
						bottom-border-1px(#f1f1f1);
						width 100%
						>a
							clearFix()
							display block
							box-sizing border-box
							padding 15px 8px
							width 100%
							.shop_left
								float left
								box-sizing: border-box
								width 23%
								height 75px
								padding-right 10px
								.shop_img
									display block
									width 100%
									height 100%
							.shop_right
								float right
								width 77%
								.shop_detail_header
									clearFix()
									width 100%
									.shop_title
										float left	
										width 200px
										color #333
										font-size 16px
										line-height 16px
										font-weight 700
									.shop_detail_ul
										float right
										margin-top 3px
										.supports
											float left
											font-size 10px
											color #999
											border 1px solid #f1f1f1
											padding 0 2px
											border-radius 2px				
								.shop_rating_order		
									clearFix()
									width 100%
									margin-top 18px
									margin-bottom 8px
									.shop_rating_order_left
										float left
										color #ff9a0d
										.rating_section
											float left
											font-size 10px
											color #ff6000
											margin-left 4px
										.order_section
											float left
											font-size 10px
											color #666
											transform scale(.8)
									.shop_rating_order_right
										float right
										font-size 0
</style>