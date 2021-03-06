# Javascript Overview
## What is JavaScript?
자바스크립트는 동적 컴퓨터 프로그래밍 언어입니다. 자바스크립트는 가볍고, 웹 페이지 분야에서 가장 흔히 쓰입니다. 구현을 통해 클라이언트 측 스크립트가 사용자와 상호작용하고 동적 페이지를 만들 수 있습니다. 자바스크립트는 객체지향적인 기능을 가진 해석된 프로그래밍언어입니다.

자바스크립트는 라이브스크립트(LiveScript)로 제일 처음 알려졌습니다. 그러나 넷스케이프에 의해 이름이 자바스크립트(JavaScript)로 바뀌었습니다. 아마 자바로부터 생겨난 흥미? 자바의 인기 때문인지?? (잘 모르겠음 possibly because of the excitement being generated by Java.) 자바스크립트는 1995년 라이브스크립트(LiveScript)라는 이름으로 넷스케이프 2.0에 처음 등장하였습니다. 자바스크립트의 범용 코어는 넷스케이프, 인터넷 익스플로러 그리고 다른 웹브라우져들에 내장되어 있습니다.

ECMA-262 는 핵심 자바스크립트 언어의 표준 버전을 정의했습니다.

* 자바스크립트는 가벼운 인터프리터 언어입니다.
* 네트워크 중심 어플리케이션을 만들기 위해 고안되었습니다.
* 자바와 비슷한 부분이 있습니다? (Complementary to and integrated with Java)
* HTML과 함께 사용할 수 있습니다? (Complementary to and integrated with HTML)
* OS 관계없이 동작합니다. (Open and cross-platform)

## Client-Side JavaScript
 클라이언트 측면에서 자바스크립트는 가장 흔히 사용하는 언어 형태입니다. 자바스크립트는 브라우저에 포함되어 있거나  해석된 코드들을 위한? (an HTML document for the code to be interpreted by the browser) HTML document에 의해 참조됩니다.

즉, 웹 페이지는 정적 HTML이 아니라 유저와 상호작용을 하거나 브라우저를 컨트롤 하는 것 그리고 동적으로 HTML 컨텐츠를 만들어내는 것들이 포함할 수 있습니다.

클라이언트 측면에서 자바스크립트의 동작방식은 기존의 전통적인  CGI 서버 쪽 스크립트보다  많은 장점들을 제공합니다. 예를 들어 사용자가 폼 영역에 유효한 이메일 주소를 입력했을 때 체크하기 위해서 자바스크립트를 사용할 수 있을 것입니다.

자바스크립트 코드는 유저가 폼을 제출하거나 진입하는 모든 것들이 유효해야만 실행되고, 웹 서버에 제출될 것입니다.

자바스크립트는 버튼 클릭, 링크 탐색 그리고 유저가 명시적이거나 암묵적으로 시작하는 다른 작업과 같은 사용자 시작 이벤트를 트랩하는 데 사용할 수 있습니다.

## Advantages of JavaScript
자바스크립트를 사용하면 얻게되는 장점은 다음과 같습니다.

*  적은 서버 상호작용? (Less server interaction)
	* 서버에 페이지를 전송하기 전에 유저의 입력을 검증할 수 있습니다. 이는 서버 트래픽을 줄여주기때문에 서버의 로드가 줄어듭니다.
*  방문자에게 즉각 피드백 전달 (Immediate feedback to the visitor)
	* 방문자들은 만약 입력 내용을 잊어버렸어도 이를 확인하기 위해 페이지가 리로드될때까지 기다리지 않아도 됩니다.
* 상호작용 증가 (Increased interactivity)
	* 여러분은 사용자가 마우스를 위로 이동하거나 키보드를 통해 어떤 인터페이스를 활성화할 때 반응하는 인터페이스를 만들 수 있습니다.
* 풍부한 인터페이스 (Richer interfaces)
	* 여러분은 자바스크립트를 사용하여드래그 앤 드롭 혹은 슬라이더 같은 아이템을 포함해 당신의 사이트 방문자들에게 풍부한 인터페이스를 제공할 수 있습니다.

## Limitations of JavaScript
우리는 자바스크립트를 완전한 프로그래밍언어로 다룰 수는 없습니다. 자바스크립트는 다음과 같이 중요한 기능이 없습니다.

* 클라이언트 측면에서 자바스크립트는 파일을 읽거나 작성할 수 없습니다. 이것은 보안상의 이유로 지속되고 있습니다.
* 자바스크립트는 네트워킹 어플리케이션에 사용할 수 없습니다. 그 이유는 그러한 지원이 불가능하기 때문입니다.
* 자바스크립트는 멀티 쓰레딩이나 멀티프로세서 기능이 없습니다.

다시 한번 말하지만 자바스크립트는 가벼운 인터프리터 언어입니다. 그러므로 여러분은 정적 HTML 페이지로 상호작용을 만들 수 있습니다. (Interactivity?)

## JavaScript Development Tools
자바스크립트의 주요 강점 중 하나는 비싼 개발 툴이 필요없다는 것입니다. 여러분은 노트패드같은 간단한 텍스트 에디터로 시작할 수 있습니다. 웹 브라우저의 컨텍스트 내부에 해석되는 언어이기 떄문에 컴파일러를 구입할 필요가 없습니다.

우리의 삶을 더 단순하게 하기 위해 (우리의 코딩을 더욱 효율적으로 하기 위해? 이 정도의 의미인가??) 다양한 벤더사들은 아주 좋은 자바스크립트 툴을 출시하고 있습니다. 그 중 일부를 소개합니다.

* Microsoft FrontPage
	* 마이크로소프트는 FrontPage라고 불리는 인기있는 HTML  에 디터를 개발해왔습니다. 또한 FrontPage는 웹 개발자들에게 interactive한 웹 사이트를 만드는데 도움을 줄 수 있는 많은 자바스크립트 도구를 제공했습니다.
* Macromedia Dreamweaver MX
	* Macromedia Dreamweaver MX는 전문적인 웹 개발자들 사이에서 매우 인기있는 HTML, 자바스크립트 에디터 입니다. 이 에디터에는 몇 개의 유용한 자바스크립트 컴포넌트가 내장되어있고, 데이터 베이스와 잘 통합됩니다. (데이터 베이스를 이 툴에서 사용할 수 있다는 말인가?  Intergrates well with databases) 그리고  XHTML 이나  XML 과 같은 새로운 표준을 따릅니다.
* Macromedia HomeSite 5
	* HomeSite5는 Macromedia의 HTML 및 자바스크립트 에디터로 개인 웹사이트를 효과적으로 관리할 수 있습니다.

## Where is JavaScript Today?
ECMAScript Edition 5 표준은 4년 동안 릴리즈된 첫번째 업데이트입니다. 자바스크립트 2.0은 ECMAScript Edition 5 표준을 따릅니다. 둘 사이의 차이점은 아주 미미합니다.

자바스크립트 2.0에 대한 상세는 다음 사이트에서 확인할 수 있습니다. http://www.ecmascript.org

오늘날 넷스케이프의 자바스크립트 그리고 마이스로소프트사의 제이스크립트는 ECMAScript 표준을 준수합니다. 그러나 두 언어 모두 표준에 속하지 않은 기능 또한 지원하고 있습니다.
