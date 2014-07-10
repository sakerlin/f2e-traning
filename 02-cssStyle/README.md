CSS coding style
==========================

* 使用reset
* 避免使用id 做為選擇器(css selector)
* 避免使用float

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

* use External Link 
* 使用class 不要寫inline style
     
