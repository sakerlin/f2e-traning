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
	- 避免使用id 做為選擇器(css selector)
	- 避免使用float
	- use External Link 
	- 使用class 不要寫inline style
     
