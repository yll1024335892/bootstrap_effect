#bootstrap的集合的适配的效果
###	test_nav1.html
![Image](https://github.com/yll1024335892/bootstrap_effect/blob/master/effect_img/test_nav1.jpg)
###	number_effect.html
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