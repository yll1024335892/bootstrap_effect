#bootstrap的集合的适配的效果
###	test_nav1.html 导航的侧滑效果
![Image](https://github.com/yll1024335892/bootstrap_effect/blob/master/effect_img/test_nav1.jpg)
###	number_effect.html 数字从0到指定数的一个插值动画
![Image](https://github.com/yll1024335892/bootstrap_effect/blob/master/effect_img/number_effect.jpg)
```
<script type="text/javascript">
	$(document).ready(function(){
		$("#btn").click(function(){
			$('.counter-value').each(function(){
					$(this).prop('Counter',0).animate({
						Counter: $(this).text()
					},{
						duration: 3500,
						easing: 'swing',
						step: function (now){
							$(this).text(Math.ceil(now));
						}
					});
				});
		});
		
	});
</script>
```
###	page_scroll_effect.html	元素滚动出页面的开始执行动画效果