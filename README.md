# sim-trad-switch
为了方便以后开发，网页需要简繁体切换用于的方法。
* 支持input、textarea的value值转化，直接调用则是返回对应文本，具体可以看demo。
* demo 页面中包含一个繁简体转化器，可以在本地直接转化。
* tips: 实例化后会对添加了定义繁简体的标签进行一次切换。
***
## update 
* 2018-04-13 : 增加debug，当前仅支持查看实例化耗时

## 使用方法
在标签的类名是添加对应的类名,简体对应的类名为sim，繁体为trad。  
如果需要进行切换请设置options.switch为ture后在按钮使用实例化后调用.changeText()进行切换。
###使用场景
* 标签内文本,支持input、textarea标签。
* 直接调用返回对应文本，实例化后调用simtradSwitch(type,string)

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
	var str = "体体体体";
		str = stSwitch.simtradSwitch("trad",str); // 切换str字符串为繁体字符串
```

# 参数
sim 	标签内文本转化为简体
trad 	标签内文本转化为繁体
# options
| options | 类型 | 默认值 | 说明 |
| ---------- |:-------:|:-------:|:------:|
| switch | boolean | false | 开启切换 |
| debug | boolean | false |　查看实例化的耗时 |
| callback | function | none | 实例化后完成的回调,返回所有的文本节点数组 |
