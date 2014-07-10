
Standar HTML
==========================
* basic html
```
    <!doctype html>
    <html lang="zh-tw">
    <head>
        <meta charset="utf-8">
        <title>Your page title</title>
    </head>
    <body>
    </body>
    </html>
```
* doctype 
    - doctype 必須是 HTML 文檔的第一行，位於 <html> 標籤之前。
    - doctype 不是 HTML 標籤；它是指示 web 瀏覽器關於頁面使用哪個 HTML 版本進行編寫的指令。 
    - html4 doctype
        ```
    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

         ```
    - html5 doctype
        ```
        <!doctype html>
         ```
* html lang
    - HTML Language Code Reference
    - 聲明網頁主要語言, 幫助瀏覽器及搜尋引擎辨視網頁

* HTML meta http-equiv
     - 提供網頁標頭關於網頁的內容屬性資訊
     - ```<meta http-equiv="屬性值" content="內容">```
     - 常見屬性  content-type、default-style、refresh
     - html4 
     ```
     <meta http-equiv="content-type" content="text/html; charset=UTF-8">
     ```
     - html5
     ```
     <meta charset="utf-8">
     ```
* codeing rule
    - tag use low case
    - attrubute embrace with double quotes
        - ex: ```<a href="xxx">link</a> ```     
    - indent use space not tab
    - 1 indent = 4 space
    - less id and class better?
    - id is unique in one page

