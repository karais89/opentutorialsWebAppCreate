# opentutorialsWebAppCreate
생활코딩 웹 애플리케이션 만들기.

프로그래밍을 처음 하는 사람이라도 다 할수 있는 수업이지만, 쉽지는 않을 것.

반응형 웹 - 사용자의 화면의 크기에 따라 적당히 컨텐츠의 모양이나 형식이 변경 되는 것도 살펴봄.

수업시간 - 20~30시간?


##웹 애플리케이션을 만드는 순서.

1. 구상.
2. 기획(계획).
3. 디자인.
4. 개발 (Development).
5. 테스트.

중요한 개념 - Start Small (처음부터 크게 만들지 말고 작게 시작해서 개선하자.)

##구상

무엇을 만들지 고민하는 과정.

생활코딩과 같은 홈페이지를 만드는 과정.

첫번째 선택 : 블로그 -> 문제(최신순 정렬)

직접구현하자라는 생각을 하게됨.

오래된 순으로 정렬.

ㅋㅋㅋ 전략 http://goo.gl/ZuuCbh

##기획

UI 모델링

* UI- UserInterface 사용자가 시스템을 제어하는 조작장치.
* 모델링 - 직접 만들기 전에 가상으로 만들어보는것. 사용자의 입장에서 동작하는 기능을 가상으로 만들어 보기.

UI 모델링이 중요한 이유! -> 커뮤니케이션

모델링 도구
* 손그림
* Pencil -> http://pencil.evolus.vn/
* balsamiq -> https://balsamiq.com (유료)
* PowerPoint


##인터넷과 웹의 역사

인터넷과 웹은 다를까요? 결론적으로 다르다.

인터넷의 안에 웹이 포함되있음 ( 인터넷이 더 넓은 개념 )

웹과 형제쯤 되는 기술들.(FTP, 이메일등..)

1960년대 - 인터넷 등장.
1990년대 - 웹 등장. 

팀버너스리 -> 웹 창시자.(HTTP, HTML 만듬)

## 서버 클라이언트(13분)

우리 수업에서 가장 큰 체계.

웹브라우저 - 클라이언트.
웹서버 - 서버.

클라이언트가 서버컴퓨터에게 **요청**함.
서버컴퓨터가 클라이언트에게 **응답**함.

클라이언트 - 갑(고객)
서버 - 을(서비스종사자)

준비물 - 웹브라우저, 웹서버(프로페셔널한..?)

웹서버를 컴퓨터에 설치해야됨.

공부할때는 한대의 컴퓨터로 가능함.(웹서버와 웹브라우저를 두개 다 설치)

웹서버 종류
* Apache(한번도 1등을 놓친적없는 웹서버 분야에서 절대강자 우리 수업은 이걸로 구축.)
* Nginx
* IIS(마이크로소프트.)

**Apache**
http://projects.apache.org/projects/http_server.html -> 여기서 설치하는게 정석이지만. 까다롭다.

**bitnami**
이걸 이용해서 한방에 설치(Apache + php + mysql)

Windows
https://bitnami.com/stack/wamp

Mac
https://bitnami.com/stack/mamp

Linux
https://bitnami.com/stack/lamp

##윈도우에 웹서버 설치

검색엔진에서 bitnami wamp 검색

용량이 꽤 큼. 120mb 정도?

프레임워크 설치 화면이 뜨는데 일단은 필요없어서 다 끔..

DB 비번 입력해줌. 123456 ?

방화벽 화면이 뜨면 - 액세스 허용

브라우저에서 localhost/index.html 입력하고엔터 -> 화면이 뜨면 정상 작동되는것.

htdocs 폴더의 index.html 을 실행해줌..

일단 기본 포트가 안되서 8000번으로 변경해줌..

localhost:8000/index.html 이런식으로 해야됨..

##서버제어

Apache, php, mysql 제어

Bitnami

Manager Servers 탭 실행이 되고 있어야됨.

Osx 나 리눅스의 경우 자동으로 꺼지니까 주의!!! 윈도우는 계속 실행되있나봄.. 중요!!

mysql 선택후 config 누르고 open log 를 누르면 로그를 볼수 있음.

apache 도 마찬가지임.

## 프로그래밍 언어(컴퓨터와 사람의 소통) - 약 3분

언어란? 사람과 사람사이의 약속

프로그래밍 언어란? 사람과 컴퓨터 사이의 약속

코드 혹은 소스라고 부름..

이렇게 코드를 작성하는 행위를 코딩.

소스 코드를 작성하는 사람을 코더 혹은 프로그래머라고 부름..

코드 -> 설계도라고 얘기할수 있음.

코드는 곧 제품이다.

코드를 작성한다 = 곧 제품을 만든다. (중요한 활동)

## HTML 이론.

웹브라우저가 웹서버에게 요청.
웹서버는 응답.(HTML 전달)

HTML 이란?
**H**ypertext -> 문서와 문서가 링크로 연결 되있다.(가장중요)
**M**arkup -> tag와 같은 의미??
**L**anguage -> 언어.

링크는 HTML 의 본질.
HTML의 본질은 웹의 본질.

Tag -> 옷을 사면 붙어져있는거 (옷을 설명해주는 정보)
HTML의 태그도 이것과 같다.

**속성**
가장 중요한 태그의 a 태그 사용법 숙지.
a -> 링크를 나타내는 태그
<a>생활코딩</a> -> 아무것도 할수 없음.

<a href="http://opentutorials.org/course/1">생활코딩</a>
생활 코딩이란 텍스트가 링크라는 사실과 href의 해당되는 주소에 연결되있다는걸 알수있음
href 는 속성명이라고 하고, href안에 들어있는값은 속성값이라고 한다.
href 는 약속이다.

**리스트**

항목화 시키는 태그
<li>html</li> li는 list의 약자.
<li>css</li>
<li>JavaScript</li>

각각의 그룹을 어떤태그로 감쌀수있음
* ul 태그 == unordered list 순서가 없는 리스트.
* ol 태그 == ordered list 순서가 있는 리스트.
* ol 태그는 자동으로 숫자가 붙음.

태그들을 또다른 태그로 묶을수있음.

* head 태그. -> 문서를 설명. 문서에 대한 정보.
* body 태그. -> 문서의 내용.
* html 태그. -> html 안쪽의 태그들이 html 문서이다.

**HTML 정리**

처음 만든사람은 팀버너스리.

누가 만들까? w3c (HTML을 체계적으로 만들기 위해서 국제기구 출범. 표준정의.)

**<!DOCTYPE html>** -> html의 문법이 아님. 이 HTML 문서가 어떤 표준안에 따라서 작성된 건지 웹 브라우저가 이해 할수 있도록 기술.
코드가 정확하게 작동하기 위해서는 이것을 통해서 명확히 표현하는게 좋다. 이 것은 html5를 의미함.

**Tag Reference**
HTML의 문법은 아주 경량이다. 100개 ~ 200개 사이일듯?
Tag를 빽빽이 하듯이 알 필요는 없을듯.
하지만 우리가 코딩을 할때는 모르는 것을 찾으면 된당.
어떤 태그가 있는지만 알면 됨.
실제로 필요할때는 찾아서 연구하면 됨.

http://dev.w3.org/html5/html-author/

http://opentutorials.org/course/1058

본질

HTML의 본질은 정보이다.
어떠한 정보를 사람도 이해하고 컴퓨터도 이해하게 태그라는 것을 이용해 규정하고 정의하는것이 HTML의 궁극적 목표다.

##HTML 실습

수업에서 할려는건 간단한 웹 사이트를 만들려는 것.

우리가 기획한 웹사이트를 정보의 형태로 만드는것 -> HTML

* h1 태그 -> 가장 큰 제목.
* h2 태그 -> 그 다음 제목.

**Semantic Web(의미가 잘 드러나는 웹)**

디자인을 담당하는 태그나 역활들이 css 로 분리되기도 함.

원시적인 웹 -> 의미론적인 웹으로.. XHTML이라는게 있었음..

현시점(HTML5)

* nav 태그 -> 내비게이션의 줄임말.. 이 태그로 감싸면 이 리스트가 네비게이션을 위한 리스트라는 걸 분명하게 이해 가능. 어떤 의미가 있지는 않음.
* header 태그 -> 이 문서의 헤더 부분에 해당되는 것이라는걸 분명히 드러낼수있음. 어떤 의미가 있지는 않음.
* article 태그 -> 본문.

**쉬어가기**

우리는 지금까지 웹서버와 웹브라우저를 이용해서 화면에 보여지는 과정을 마침.

초기의 웹을 복원했다.. 초기의 웹은 이정도의 기능성을 가지고 있음.

시간이 지날 수록 훨 씬더 많은 사람들이 웹을 함.

하지만 시간이 지날 수록 점점 복잡해짐.

강력해진만큼 복잡해졌다.

본질에 집중하자.

갈림길에 서있음.. 우리가 선택할수있는 두가지의 길이 있음..

웹브라우저(클라이언트사이드 테크놀로지.)
* HTML
* CSS
* JavaScript

웹서버(서버사이드 테크놀로지.)
* PHP
* MySQL

실제로 현업에서는 클라이언트 엔지니어가 있고 서버 엔지니어가 있음.(규모가 커지면..)

서버 사이드 기술들은 아무래도 낯설긴함(일반인들기준으로)

순서

클라이언트 -> 서버

## 개발도구

도구의 필요성.. ( 삽과 포크레인같음) 포크레인은 강력하지만 배우는데 오래걸림.

버전 관리 시스템(Version Control System) - 여러분이 작성한 코드를 서버에 안전하게 저장. 조금 어려움.. 

**버전 관리 시스템**
* git - 가장 유망한 버전관리 시스템.
* svn
* Mecurial

git - http://opentutorials/org/course/1492

**코드편집기(Editor)**

에디터는 포크레인 같음. 에디터를 사용하면 훨씬 더 빠르게 작업 할 수 있음.

우리 수업에 사용할 에디터는 github의 atom을 사용할 예정.

우리 수업에서 아톰 에디터는 필수 사항이 아니다. 메모장이나 텍스트 에디터를 사용해도 아무 문제 없음.

**에디터 종류**
* Aptana
* Sublime Text
* Brackets

더 좋은 에디터를 선택하는 건 엔지니어가 당연히 추구해야 될 **목적**이다.

생산성을 높이는데 노력하자.

아톰 : https://atom.io/

아톰에 대한 상세한 사용법은 다음 수업을 참고해주세요. https://opentutorials.org/module/1579

아톰 설치에 문제가 있는 분은 sublime text를 추천합니다. https://opentutorials.org/course/671/3595

현재 저는 visual code를 사용. https://www.visualstudio.com/ko-kr/products/code-vs.aspx

visual code 는 emmet 를 이미 내장하고 있음.

**윈도우에 아톰 설치** (50초)

다운로드를 누르고 설치. 끝 참 간단하죠?

**아톰 사용법**

File - Open Folder 를 선택해서 우리가 선택할 폴더를 선택하면 쉽게 작성할수 있음. htdocs를 선택.

**장점**
* 더블클릭하면 바로 탭으로 열림. 탭 전환을 통해 빠르게 파일을 수정할 수 있다.
* 알록달록하다. (가독석 향상) - 코드 하이라이트??
* 줄번호
* 플러그인 존재.(확장기능) - 기본 기능 이외의 기능.
* 화면 분할 가능.

아톰의 확장기능중 emmet 설치. - 최고의 확장기능.. html 작성시 거의 필수..

**emmet**
* 코드를 작성하는 걸 도와주는 환상적인 확장기능
새로운 도구가 나오면 개발자들은 마음이 설레임. ?? 이게 낙인 사람이들 많음
* emmet cheat sheet http://docs.emmet.io/cheat-sheet/

신났네..

li*3>a 탭 같은거는 신세계인듯.
ol>li*3>a 이런거..

상당히 빠르게 편집 가능.
Ctrl를 누르고 있는 상태에서 드래그. 멀티 셀렉션이 됨... 그리고 타자를 치면 한번에 바뀔 수 있음.
아주 강력크한 기능..
생산성이 비약적으로 향상.

## CSS 이론

**CSS의 기본문법**

HTML은 못생겼음.. 

정보를 아름답게 표현하는 언어는 CSS

**C**ascading **S**tyle **S**heet

STYLE - 주목

HTML + CSS

CSS는 HTML과 완전히 별개의 언어지만 HTML을 떠날 수 없음.

처음에는 HTML 밖에 없었지만.. HTML이 정보에 집중하게 하기 위해.. CSS가 그 일을 담당.

HTML = 정보

CSS = 디자인

style 태그

**박스모델**

박스모델이 중요함.

브라우저에서 요소 검사. 여기서 이것저것 만져보면 대충이라도 알수 있음.

구글 개발자 도구는 브라우저 상에서 실시간으로 수치를 바꿔가면서 시각적으로 아름다운가 등을 확인 할수 있음.

크롬 개발자 도구 : https://opentutorials.org/course/580

**float**

css의 효과 중요한 문법은 아니지만 다음 수업에서 사용할 내용이기 때문에 미리 소개.

웹 페이지의 레이아웃을 디자인 할때 중요하게 사용됨


## css 실습.

nav - 컨텐츠 폭을 200px, float 속성으로 본문이 오른쪽에 위치하도록. 오른쪽 테두리.
article - float:left, 적절한 여백.

모든 페이지가 같은 컨셉의 레이아웃으로 나오는게 목표.

개선사항.. -> css 파일로 관리. 중복의 제거..

css 후속강의 : http://opentutorials.org/course/45

정리 
htm = 정보.
css = 디자인.

## 복습과 수업 예고

PHP나 Javascript

PHP는 하나의 html 파일을 만들수 있다.

## JavaScript vs PHP

둘다 프로그래밍 언어이고, 둘다 비슷비슷함.

같이 배우면 시간이 빠르게 단축됨.

자바스크립트와 PHP 는 대단히 미묘한 관계

JavaScript - 클라이언트
PHP - 서버

두개의 언어는 협력적인 관계이기도 함. ( 하지만 Node.js 가 등장했지...)

* HTML, CSS - 정적인 언어(한번 작성하면 바뀌지 않음)
* JavaScript, PHP - 동적인 언어(사용자가 버튼을 누르면 어떤일이 일어나고, 어떤 정보를 입력하면 저장되고..)

CGI - PHP, PERL, JSP 등..

## 웹페이지에 코드 삽입하기.

두개의 언어를 동시에 익힐거임.(php, javascript)

**삽입**

기본적으로 php 파일은 html 과 똑같이 동작함.

PHP 인터프리터가 소스코드를 해석한 결과를 웹서버에 전달하기 때문에.. 

<?php echo 10+10; ?> -> 20 으로 변경된 값을 웹서버가 받고 그 내용을 웹 브라우저에게 전달하기 때문에 php 코드를 볼수없음.

하지만 자바스크립트는 웹서버에서 실행되는 언어이기 때문에.. 코드를 볼수 있음.

PHP는 서버에서 처리된 결과이고. (서버)

자바스크립트는 웹 브라우저에서 처리된 결과이다. (클라이언트)

## 데이터타입과 연산자

문자를 표기하는 방법.

큰따옴표로 시작 

숫자를 표현하고 싶으면 큰따옴표로 쓰면안됨.

"1000000" = 문자 십만임..

문자를 더할때 PHP 는 (.)점을 사용..

자바스크립트는 + 연산자 사용.

## 디버깅

**디버그**

방법에 대한 얘기보다는 어디에서 오류가 생겼는지 찾는 방법..(나는 방법을 알고 싶은뎅.)

자바스크릡트:  웹브라우저에서 도구더보기 - 콘솔 창을 확인해보면 에러 로그가 나옴
php : apache2 폴더의 logs 의 error.txt 확인.

보충수업?
php에 에러가 있을때 화면에 에러가 표시하게 하는것.
C:\Bitnami\wampstack-5.5.30-0\php\php.ini 파일을 열어서..
display_errors = Off 을 On 으로 변경.
Bitnami 매니저 실행하고 아파치 재실행.
PHP는 아파치라는 웹서버에 내부적인 부품과 같은 형태로 동작하고 있는 방식?
디테일한 얘기는 몰라도 됨.

## 변수

바뀔수 있는 값.

자바 : name = "이고잉";

PHP : $name = "이고잉";

변수를 쓰는 이유? 프로그램을 최대한 변경하지 않기 위해.

## 비교

대소 관계를 판단.. 같다 다르다.

==, !=, >, < 등

true, false 를 Boolean 이라고함(블리언)

## 조건문

굉장히 중요한 부분.

컴퓨터의 영역.

어떠한 상황에 따라 이렇게도 되고 저렇게도 되는 것.

자바스크립트, PHP 아래와 같음.(동일)

<pre>

if(true/false) {
    
    // true 인 경우 여기 실행.

}else {

    // false 인 경우 여기 실행.

}

</pre>

## 로그인 기능 만들기.

지금까지 배운거 중간 정리.

조건문이 중요.

## 반복문

반복적인 작업.

사람은 반복적인 작업을 잘 못함.

기계는 반복을 좋아함.

조건문이 기계를 똑똑하게 하는 것이라면..

반복문은 무언가 반복적인 작업을 해서 많은 일을 처리하는 작업.

여기까지 하면 가장 중요하다고 하는 것들은 다 배웠다고 생각하면 됨.

자바스크립트와 PHP 반복문 똑같음.

<pre>
while(true/false) {
    // true이면 계속 반복.
    
}
</pre>

## 배열

영어로 Array

어떤 정보를 담는 그릇.

지금까지 살펴본 정보를 담는 그릇은 변수였음.

배열은 변수와 비슷하면서 다르다.

변수안에는 하나의 값만 담을 수 있지만 배열 안에는 서로 연관되있는 여러 정보들을 하나의 배열이라는 그릇에 담아서 체계적으로 관리 할수 있는 도구이다.

<pre>
// JavaScript
list = new Array("one", "two", "three");

list[0];

// PHP
$list = array("one", "two", "three");

$list[0];
</pre>

배열을 쓰는 이유? 그룹핑??

## 배열과 반복문

배열과 반복문은 바늘과 실 같은 존재.

## 함수

수학시간에 배우죠..

함수는 굉장히 중요한 도구다..

프로그래밍을 하면 수학을 좀더 구체적인 느낌으로 배울 수 있다..

우리는 수학을 못하는 사람이 아니고 잘할 사람들이다??

수학시간의 함수랑 느낌은 다르지만 본질은 같을 것이다..

<pre>
// JavaScript
function function_name() {
}

function_name();

// PHP
function function_name() {
}

function_name();
</pre>

JavaScript 나 PHP 나 거의 똑같음..

아는 만큼 보인다.

# UI vs API

UI - **U**ser **I**nterface

API - **A**pplication **P**rogramming **I**nterface

Interface - 사람과 사람이 서로 교류할때 사용되는 가장 기본적인 도구인 **언어** 마찬가지임.

사용자가 직접 조작하는 인터페이스를 UI 라고 부름.

애플리케이션이 무언가를 하기 위해 프로그래밍 적으로 그 애플리케이션이 돌아가는 시스템에게 전달하는 명령을 API 라고함.

**API 전성시대!**

과거에는 API를 제공하는 시스템이 운영체제 정도가 있었음.

웹브라우저가 발달하면 수많은 웹 애플리케이션이 만들어지고..

굉장히 많은 사람들이 사용하는 서비스이고.. 무엇보다 중요한건 스스로 API 를 제공함.(facebook, google plus, twitter)

여기서 끝이 아니고.. 스마트 폰이 등장하면서 스마트폰이라는 플랫폼은 API 를 제공.

스마트 폰 뿐만 아니라 수 많은 디바이스도 API 를 제공.

API의 폭발적 증가 + 쉬워진 프로그래밍 (~~개나 소나 다하는..~~)