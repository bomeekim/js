# JavaScript Syntax
자바스크립트는 자바스크립트 선언문을 사용하여 구현할 수 있습니다. 웹 페이지 내에 \<script> ... \</script> HTML 태그 안에 대체됩니다. 여러분은 자바스크립트가 포함된 \<script> 태그를 웹 페이지 내 어디에나 배치할 수 있지만 일반적으로는 \<head> 태그 내에 두는 것을 추천합니다. \<script> 태그는 브라우저 프로그램에게 이 태그 사이에 포함된 모든 텍스트를 스크립트로 해석하기 시작한다고 알려줍니다. 자바스크립트의 간단한 구문은 다음과 같습니다.
```html
<script>
   JavaScript code
</script>
```


스크립트 태그는 두 개의 중요한 속성을 가지고 있습니다.

* Language
	* 이 특성은 여러분이 사용하는 스크립트 언어가 무엇인지를 명시합니다. 일반적으로 이 값은 자바스크립트가 될 것입니다. 그러나 최신 버전의 HTML (및 그 후속인 XHTML)에서는 이 속성의 사용을 단계적으로 중단했습니다.
* Type
	* 이 속성은 현재 사용하는 스크립트 언어를 나타내는데 권장되며 해당 값은 'text/javascript'로 설정해야 합니다.

자바스크립트 세그먼트는 다음과 같습니다.
```html
<script language = "javascript" type = "text/javascript">
   JavaScript code
</script>
```


## Your First JavaScript Code
"Hello World"를 프린트하는 샘플 예제를 가져왔습니다. 예제에서는 자바스크립트 코드를 둘러싸고있는 HTML 주석을 추가했습니다. 자바스크립트를 지원하지 않는 브라우저에서 코드를 저장하기 위한 것입니다. 이 주석은 "-->" 으로 끝납니다. 여기서 ""은 자바스크립트에서 주석을 의미합니다. 브라우저가 HTML 주석의 끝을 자바스크립트 코드의 일부로 읽지 못하게 하기 위해 이를 추가합니다. 다음으로 HTML 문서에 문자열을 쓰는 document.write 함수가 호출됩니다. 
이 함수는 text, HTML 혹은 둘 다 작성하는 데 사용됩니다. 다음 코드를 보겠습니다.
```html
<html>
   <body>   
      <script language = "javascript" type = "text/javascript">
         <!--
            document.write("Hello World!")
         //-->
      </script>      
   </body>
</html>
```

이 코드의 결과는 다음과 같습니다.
`Hello World!`

## Whitespace and Line Breaks
자바스크립트는 자바스크립트 프로그램 내 나타나는공백, 탭, 새 줄을 무시합니다. 여러분은 여러분의 프로그램에 자유롭게 공백, 탭 그리고 새 줄을 사용할 수 있습니다. 그리고 프로그램을 깔끔하고 일관성있게 포맷하고 들여쓰기 하여 코드를 쉽게 읽고 이해할 수 있습니다.

## Semicolons are Optional
자바스크립트에서 간단한 코드한 줄 에는 일반적으로 C, C++ 및 자바와 같이 세미콜론 문자가 따릅니다. 그러나 자바스크립트에서는 statement가 한 줄 씩 분리되어 있는 경우 세미콜론을 생략할 수 있습니다. 예를 들어 아래 코드는 세미콜론 없이 작성될 수 있습니다.
```html
<script language = "javascript" type = "text/javascript">
   <!--
      var1 = 10
      var2 = 20
   //-->
</script>
```

그렇지만 아래 처럼 하나의 줄에 작성할 때는 반드시 세미콜론을 사용해야 합니다.
```html
<script language = "javascript" type = "text/javascript">
   <!--
      var1 = 10; var2 = 20;
   //-->
</script>
```

**Note** - 세미콜론을 사용하는 것은 좋은 프로그래밍 습관입니다.

## Case Sensitivity
자바스크립트는 대소문자를 구분하는 언어입니다. 즉, 키워드, 변수, 함수이름 그리고 다른 기타 식별자 등은 반드시 항상 일정한 대문자로 입력해야 합니다.
그러므로 식별자 Time과 TIME은 자바스크립트 내에서 다른 의미를 가져다줄 수 있습니다.

**Note** - 자바스크립트에서 변수와 함수명을 작성할 때는 주의해야합니다.

## Comments in JavaScript
자바스크립트는 C와 C++ 스타일 주석을 지원합니다. 

*  와 해당 줄의 끝 사이의 텍스트는 주석으로 취급되고 자바스크립트에 의해 무시됩니다.
* _*와 *_ 사이에 있는 텍스트는 주석으로 취급됩니다. 이 형태는 여러 줄에 걸쳐 있을 수 있습니다.
* 또한 자바스크립트는 HTML 주석의 시작 시퀀스 <!-- 알고 있습니다. 자바스크립트에서는 이러한 것을  주석과 마찬가지로 한 줄의 주석으로 처리합니다.
* HTML 주석의 닫기 시퀀스 --> 는 자바스크립트에서 인식되지 않으므로 반드시 //--> 로 작성해야합니다.

### Example
다음 예제는 자바스크립트에서 주석을 사용하는 방법입니다.
```html
<script language = "javascript" type = "text/javascript">
   <!--
      // This is a comment. It is similar to comments in C++
   
      /*
      * This is a multi-line comment in JavaScript
      * It is very similar to comments in C Programming
      */
   //-->
</script>
```
