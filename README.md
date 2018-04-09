# sim-trad-switch
为了方便以后开发，网页需要简繁体切换用于的方法。
实例化后会对添加了定义繁简体的标签进行一次切换。

## 使用方法
在标签的类名是添加对应的类名,简体对应的类名为sim，繁体为trad。
如果需要进行切换options.switch为ture，在按钮使用实例化后stSwitch.changeText()进行切换。


# html
```
	<section class="sim">
		文字内容
	</section>
```
# js
```
	var stSwitch = new stSwitch({
		switch: true
	});
	stSwitch.changeText();	//切换繁简体
```

# 参数
sim 	标签内文本转化为简体
trad 	标签内文本转化为繁体
# options
switch [boolean] 是否开启切换