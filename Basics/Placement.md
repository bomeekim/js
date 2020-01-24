# JavaScript Placement in HTML File
HTML Document 에는 자바스크립트 코드를 어디에든 넣을 수 있습니다. HTML 파일 내에서 자바스크립트를 포함시키는 방법 중 가장 선호하는 방법은 다음과 같습니다.

* `<head>...</head>` 안에 스크립트 넣기
* `<body>...</body>` 안에 스크립트 넣기
*  `<body>...</body>`그리고 `<head>...</head>`안에 각각 스크립트 넣기
* 외부파일에 스크립트를 작성하고 `<head>...</head>`부분에 포함시키기

이번 섹션에서는 각각의 다른 방법으로 HTML 파일에 자바스크립트를 넣는 방법에 대해 알아보겠습니다.

## JavaScript in <head>...</head> section
여러분이 사용자가 어딘가를 눌렀을 때처럼 이벤트를 실행하려는 스크립트를 구현하려면 다음과 같이 헤드 부분에 스크립트를 두어야합니다.

```html
<html>
   <head>      
      <script type = "text/javascript">
         <!--
            function sayHello() {
               alert("Hello World")
            }
         //-->
      </script>     
   </head>
   
   <body>
      <input type = "button" onclick = "sayHello()" value = "Say Hello" />
   </body>  
</html>
```

위 코드의 실행 결과는 [실행예제 링크](https://www.tutorialspoint.com/online_javascript_editor.php)에서 직접 확인해볼 수 있습니다.

## JavaScript in <body>...</body> section
페이지가 로드되었을 때 실행할 스크립트가 필요하여 페이지의 내용을 스크립트가 생성해야하는 경, 스크립트는 <body> 부분에 들어갑니다. 이 경우에는 자바스크립트로 함수를 만들지 않아도 됩니다. 아래 코드를 보겠습니다.

```html
<html>
   <head>
   </head>
   
   <body>
      <script type = "text/javascript">
         <!--
            document.write("Hello World")
         //-->
      </script>
      
      <p>This is web page body </p>
   </body>
</html>
```

다음은 위 코드의 실행 결과입니다.
```
Hello Wold
This is web page body
```

[실행예제 링크](https://www.tutorialspoint.com/online_javascript_editor.php)에서 직접 확인해볼 수 있습니다.

## JavaScript in <body> and <head> Sections
다음과 같이 자바스크립트 코드를 <body> 와 <head> 부분에 각각 놓을 수도 있습니다.

```html
<html>
   <head>
      <script type = "text/javascript">
         <!--
            function sayHello() {
               alert("Hello World")
            }
         //-->
      </script>
   </head>
   
   <body>
      <script type = "text/javascript">
         <!--
            document.write("Hello World")
         //-->
      </script>
      
      <input type = "button" onclick = "sayHello()" value = "Say Hello" />
   </body>
</html>
```

위 코드의 실행 결과는 [실행예제 링크](https://www.tutorialspoint.com/online_javascript_editor.php)에서 직접 확인해볼 수 있습니다.

## JavaScript in External File
여러분이 자바스크립트로 좀 더 광범위하게 작업하기 시작하면 사이트에서 여러 페이지에 동일한 코드들을 재사용해야하는 경우가 생길 것입니다.

여러 개의 HTML 파일에서 동일한 코드를 유지하는 것이 제한되지는 않습니다. 그러나 <script></script> 태그는 외부 파일에 자바스크립트를 저장한 다음 여러분이 만든 HTML 파일에 포함해 사용할 수 있는 메커니즘을 제공합니다.

다음은 어떻게 외부 자바스크립트 파일을 스크립트 태그와  src  속성을 이용해 여러분이 만든 HTML에 포함시는지를 보여주는 예제입니다.

```html
<html>
   <head>
      <script type = "text/javascript" src = "filename.js" ></script>
   </head>
   
   <body>
      .......
   </body>
</html>
```

자바스크립트 외부 파일 소스를 사용하기 위해서는 '.js'확장자를 가지는 간단한 텍스트 파일에 자바스크립트 코드를 작성해야합니다. 그런 다음 위에보이는 것과 같이 파일을 포함시키면 됩니다.

예를 들어 filename.js 파일에 다음의 컨텐츠를 넣은 뒤에 이 파일을 포함시키고, HTML 라일에서 sayHello 함수를 사용하면 됩니다.
```javascript
function sayHello() {
   alert("Hello World")
}
```
