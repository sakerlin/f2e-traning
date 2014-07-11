CSS coding style
==========================
* css
	- Cascading Style Sheets (簡寫CSS) 又稱串樣式列表、階層式樣式表檔案
	- 參考<a href="http://zh.wikipedia.org/wiki/%E5%B1%82%E5%8F%A0%E6%A0%B7%E5%BC%8F%E8%A1%A8">wiki</a>
	- css format 
	```
		<selector> {
			<property> : <value>;
		}
	```
	- ex:
	```
		.link {
			color: #f00;
		}
	```
* css selector
	- class : 
	``` 
		.link {  
			color: #f00 ;
		}
		<a class="link" href="xx">link</a>
	```
	- html tag :
	```
		a{
			color: #f00 ;
		}
		<a href="xx">link</a>
	```
	- id :
	```
		#alink{
			color: #f00 ;
		}
		<a id="alink" href="xx">link</a>
		
	```
	- attribute :
	```
		[href] {
			color: #f00 ;
		}
		[href="xx"] {
			color:#00f;
		}
		<a id="alink" href="xx">link</a>
	```
	- 串接
	```
		.item a{ 
			color: #f00;
		}
		<div class="item">
			<a class="" href="xx">link</a>
		</div>
	```
* css color value
	- #{RGB}
	- hex or string
	- hex : #336699, #f00 ...
	- string : red, white, black... <a href="http://www.w3schools.com/cssref/css_colornames.asp">參考 w3c school</a>
	
* css 屬性縮寫
	- ex: 
```
	.block{
		margin-top: 10px;
		margin-right: 10px;
		margin-bottom: 10px;
		margin-left: 10px;
	}
    =>
	.block {
		margin: 10px;
	},
	
	.block2{
		margin-top: 10px;
		margin-right: 20px;
		margin-bottom: 10px;
		margin-left: 20px;
	}
    =>
	.block2{
		margin: 10px 20px;
	},
	.block3{
		margin-top: 10px;
		margin-right: 20px;
		margin-bottom: 30px;
		margin-left: 40px;
	}
    =>
	.block3{
		margin: 10px 20px 30px 40px;
	}
	
	margin: top right bottom left
```
* css background 屬性
	- background-color
		```
			.bg { background-color: #f00; }
		```
	- background-image
		```
			.bg { background-image: url(image.png); }
		```
	- background-repeat
		
		```
			.bg { background-image: no-repeat; }
			.bg { background-image: repeat-x; }
			.bg { background-image: repeat-y; }
		```
	- background-position <a href="http://www.w3school.com.cn/cssref/pr_background-position.asp">參考w3c school</a>
			<table class="dataintable">
<tbody><tr>
<th>值</th>
<th>描述</th>
</tr>

<tr>
<td>
<ul>
<li>top left</li>
<li>top center</li>
<li>top right</li>
<li>center left</li>
<li>center center</li>
<li>center right</li>
<li>bottom left</li>
<li>bottom center</li>
<li>bottom right</li>
</ul>
</td>
<td>
<p>如果您僅規定了一個關鍵詞，那麼第二個值將是"center"。</p>
<p>默認值：0% 0%。</p>
</td>
</tr>

<tr>
<td>x% y%</td>
<td>
<p>第一個值是水平位置，第二個值是垂直位置。</p>
<p>左上角是 0% 0%。右下角是 100% 100%。</p>
<p>如果您僅規定了一個值，另一個值將是 50%。</p>
</td>
</tr>

<tr>
<td>xpos ypos</td>
<td>
<p>第一個值是水平位置，第二個值是垂直位置。</p>
<p>左上角是 0 0。單位是像素 (0px 0px) 或任何其他的 CSS 單位。</p>
<p>如果您僅規定了一個值，另一個值將是50%。</p>
<p>您可以混合使用 % 和 position 值。</p>
</td>
</tr>
</tbody></table>


* css 權重
	- selector 串接多的 覆蓋串的少的
		```
		div a{} > a{}
		```
	- selector 相同後面覆蓋前面
		```
		a{ color:#f00;}
		a{ color:#0f0;}
		```
	- inline > Embed > External Link = import
	- <a href="http://cssspecificity.com/">參考 css specificity</a>
	- <a href="">權重計算機</a>

* 套用css 的方法
    - inline 
    ```
    <a href="xxx" style="color: #ccc">link</a>
    ```
    - Embed
    ```
    <style>
        .link { color: #ccc}
    </style>
    <a href="xxx" class="link">link</a>
    ```
    - External Link
    ```
    <link rel="stylesheet" type="text/css" href="cssfonts-min.css">
    <a href="xxx" class="link">link</a>
    ```
    - import
    ```
    <style> 
        @import url(http://www.mysite.com/style.css); 
    </style>
    <a href="xxx" class="link">link</a>
    ```
*  ```<style>``` 的位置
    ```
    <!doctype html>
    <html lang="zh-tw">
    <head>
	    <meta content="text/html; charset=utf-8" http-equiv="Content-Type">
	    <meta name = "viewport" content = "width = device-width">
	    <link rel="stylesheet" type="text/css" href="">	
        <style>
            .someclass{ ...}
	    </style>
	    <title>title</title>
	</head> 
    <body>
 
    </body>
    </html>
    ```

* coding rules
	- 使用reset
	- 避免使用id 做為 css selector (css 重用性)
	- 避免使用float
	- use External Link 
	- 使用class 不要寫inline style
	- 為容易閱讀及方便diff 請每個屬性換行
	- 使用module name space 避免混淆
     
