# jQuery轻量级提示框弹出层

jQuery轻量级提示框弹出层是一款具有自动关闭功能，时间可控制，也可用代码强制关闭，具有可配置性的默认参数。

## 使用方法

### 直接按默认打开
```javascript
$.Prompt();
```

### 设置提示内容

```javascript
$.Prompt("欢迎光临本站!");
```



### 设置关闭的时间为4s

```javascript
$.Prompt("欢迎光临本站!4S",4000);
```



### 设置自动关闭时间为100s，然后在2s后强制关闭

```javascript
$.Prompt("欢迎光临本站!2S",100000);
setTimeout(function(){
	$.Prompt({close:true});
},2000);	
```



### 修改默认参数后，不带参数打开

```javascript
var def = {
	content:"欢迎光临本站",
	time:1000
}
$.Prompt(def);
$.Prompt();
```

