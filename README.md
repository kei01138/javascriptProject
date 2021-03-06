# javascriptProject
### 자바스크립트 프로젝트북
##### 실무에 적합한 9가지 프로젝트로 배우는 웹 프로그래밍

###### 섹션 별로 펼쳐서 보세요

<details><summary>배경지식</summary>
<p>

##### HTML을 먼저 불러온 후 자바스크립트를 실행한다.   

> 문서 하단 <body> 태그가 끝나기 전에 작성한다.
> /basicSyntax/internalJS.html

##### 성능 향상을 위해 CSS3와 자바스트립트 간의 역활 분담을 해야한다.

> CSS3의 그래픽 처리는 하드웨어 가속으로 작동해 자바스크립트의 그래픽 처리 보다 현저히 부드럽다.
> /basicSyntax/css3&jQuery.html  

</p>
</details>


<details><summary>Basic Syntax</summary>
<p>

##### 동적 타입의 변수 선언    

> 특정 값을 입력하는 순간 타입이 자동으로 선언된다.
> /basicSyntax/jsDynamicTypes.html


##### UX/Ui 기본

> document.write 함수 사용  
> /basicSyntax/multipleTable.html  

> document.getElementById 함수 사용  
> /basicSyntax/nickBackground.html

> eventhandler 응용
> /basicSyntax/NightorDay.html

##### for

> /basicSyntax/forloop.html


##### function

> /basicSyntax/functionJS.html

##### callback

> 많이 사용되는 콜백 함수다 익숙해지자
> /basicSyntax/callbackJS.html

##### array

> /basicSyntax/arrayJS.html

##### object

> /basicSyntax/objectJS.html
</p>
</details>



<details><summary>DOM</summary>
<p>

##### single Selector  

> document.getElementById(id명): 아이디 사용해 문서 객체(요소) 선택  
> document.querySelector(CSS 선택자): CSS 선택자를 사용하는 방식(IE 8 이상)    
> /DOM/singleSelector.html  

##### multiple Selector

> document.getElementsByTagName(요소명): 태크명으로 여러 문서 객체 선택  
> document.getElementsByClassName(클래스명): 클래스명으로 여러 문서 객체 선택(IE 9 이상)  
> document.querySelectorAll(CSS 선택자): CSS 선택자로 여러 문서 객체 전달(IE 9 이상)  
> /DOM/multipleSelector.html  

##### 텍스트 조작

> DOM.innerText: 요소 내부의 텍스트를 읽거나 변경  
> DOM.innerHTML: 요소 내부의 HTML 형식을 읽거나 변경  
> /DOM/innerText&innerHTML.html  

##### Style 객체

> 요소.style.backgroundImage: background-image   
> 요소.style.backgroundColor: background-color   
> 요소.style.listStyle: list-style   
> /DOM/styleObject.html  

##### 속성 조작

> setAttribute(속성명, 값): 속성값 설정  
> getAttribute(속성명): 속성값 읽기  
> removeAttribute(속성명): 속성 제거  
> /DOM/setAttribute.html  
> /DOM/getAttribute.html  
> /DOM/removeAttribute.html  

##### 응용

> make div Red or Blue  
> /DOM/red&blueButton.html  

</p>
</details>

<details><summary>이벤트 제어</summary>
<p>

##### 마우스와 키보드 이벤트  

```

    <요소 이벤트 핸들러 속성 = 'javaScript 명령어'>  

    <a href="http://www.google.com" onclick ="alert('구글로 이동합니다.')">
      구글  
    </a>

```  

> onclick           : 마우스를 클릭할 때  
> onmouseover       : 요소안에 마우스가 들어갔을 때  
> onmouseout        : 요소에서 마우스가 벗어났을 때  
> onkeydown         : 키보드를 입력할 때  
> onkeyup           : 키를 눌렀다 놓을 때  
> onfocus, onblur   : 요소가 선택됐거나 해제됐을 때  
> onsubmit          : 폼 전송 이벤트가 발생했을 때  


##### 이벤트 핸들러

```
    (문서 객체).(이벤트 속성명) = function(){}
```
> 자바스크립트가 문서를 조작하려고 할 경우 문서보다 먼저 작성하면 안됩니다.  
> /eventControl/beforeEventHandler.html  
> /eventControl/afterEventHandler.html

##### 이벤트 객체와 this

> this는 이벤트가 발생한 객체 자신을 의미합니다.  
> 사용자가 클릭한 요소의 위치를 반환해주기 때문에 상대적인 지정 방식으로 자주 사용합니다.  
> /eventControl/thisEventHandler.html

##### 이벤트 리스너

> 이벤트 핸들러는 객체에 속성으로 이벤트를 지정하는 방식
>> 요소당 하나의 이벤트  
> /eventControl/eventHandler.html   

> 이벤트 리스너는 메서드 방식입니다.    
>> 요소당 여러 개의 순차적인 이벤트 처리 가능
> /eventControl/eventListener.html

```
    (문서 객체).addEventListener(이벤트 타입, 리스너);
```

> 이벤트 타입: 이벤트 속성을 지정합니다. 앞에 on을 붙이지 않습니다.  
> 리스너: 이벤트가 발생할 때 호출할 함수 또는 메서드를 지정합니다.   

##### hover 구현

> 자바스크립트에 hover 이벤트가 따로 있지 않아  
> mouseover와 mouseout 이벤트를 조합해 구현할 수 있다.  
> /eventControl/hoverForJS.html

##### submit 이벤트와 기본 동작 방지

> 기본 이벤트를 차단할 수 있다. preventDefault() 사용  
>  /eventControl/submitWithPreventDefault.html  

##### 터치 이벤트

> touchstart: 화면을 건드렸을 때  
> touchend: 화면에서 손을 떼었을 때  
> touchmove: 화면에서 터치로로 이동 중일때  
> /eventControl/touchEvent.html

##### 이벤트 바인딩

> 바인딩이란 함수를 외부에 작성하고 내부에는 함수명만 작성하는 방식  
> 처리는 동일합니다  
> /eventControl/eventBinding.html  

##### 드래그 앤 드롭 구현

> /eventControl/touchEvent.html 참조해 만들었습니다.  
> clientX: 브라우저 화면을 기준으로 한 X 좌표  
> clientY: 브라우저 화면을 기준으로 한 Y 좌표  
> touchmove: 화면에서 터치로 이동 중일 때  
> /eventControl/drag&drop.html  


</p>
</details>

<details><summary>워밍업: 프로그래밍 도전하기</summary>
<p>

##### 구구단 출력 애플리케이션

> prompt()  

```
  // text는 prompt 상자에 표시되는 질문 텍스트
  // defaultText는 옵션 항목으로 글상자에 표시됩니다
  prompt(text, defaultText)
```
> isNaN()
```
  // isNaN() 메서드는 매개 변수에 입력된 값이 문자인지 판단합니다.
  var str = 'hello';
  var num = 3;
  document.write(isNaN(str) + '<br>');  // true
  document.write(isNaN(num) + '<br>');  // false
```

##### 작업 목록 애플리케이션

> 이벤트 리스너    

###### appList.html

> 목록을 추가하기 전까지 작동함
> 목록을 추가하면 작동 안함
###### appList2.html
> ul에 클래스를 먹여서 목록을 추가해도 작동함

### 깨달음
> 이벤트 리스너는 정적인 문서 객체만 제어할 수 있으며,  
> 자바스크립트에서 동적으로 추가된 요소는 바로 인식하지 못합니다.  
> 이 경우 이벤트 핸들러와 event.target 속성으로 동적으로 생성된 문서 객체를 알아낼 수 있습니다.  

</p>
</details>


<details><summary>jQuery</summary>
<p>

##### jQuery 추가하기  

> 제이쿼리 파일은 사용자가 작성한 자바스크립트 코드(app.js)보다 반드시 먼저 위치해야한다.  
> 압축 버전(*.min.js)과 비압축 버전(*.js)이 있다.  

```
    <head>
        <title>jQuery</title>
        <script src="jquery.min.js"></script>
        <script src="app.js"></script>
    </head>
```

> CDN(Content Delivery Network) 서비스로 추가하기  
```
    <head>
        <title>jQuery</title>
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
        <script src="app.js"></script>
    </head>
```

> 기본 문법
```
    $(선택자).메서드;
    $(객체).메서드;
```

##### 객체와 메서드
```
    $(document).ready();
```

> jQuery로 코드를 작성할 때 가장 먼저 작성하는 함수이며  
> 문서 로딩 완료 후 함수 안의 명령어를 실행합니다.  
> 네이티브 자바스크립트의 window.onload 이벤트 핸들러와 같은 역활입니다.   
> /jQuery/object&Method.html

##### 선택자

###### CSS 선택자 사용해 제어하자
> /jQuery/selector.html

###### 필터 메서드 사용하자
> .eq(): 특정 순서의 요소를 선택합니다. 매개변수의 배열값으로 지정합니다.    
> .filter(): 매개 변수에 지정한 이름의 형제 요소를 선택합니다.  
> .first(): 첫번째 요소를 선택합니다.  
> .last(): 마지막 요소를 선택합니다.  
> .has(): 매개변수에 지정된 요소를 자식 요소로 포함한 요소를 선택합니다.  
>> /jQuery/filterMethod.html
###### DOM 탐색 메서드
> .parent(): 직계 부모 요소를 선택합니다.  
> .parents(): 매개 변수에 지정한 이름의 조상을 탐색합니다.   
> .children(): 매개 변수에 지정한 후손을 선택합니다.  
> .find(): 하위 후손 노드를 찾아 선택합니다.  
> .siblings(): 매개 변수에 지정한 형제 요소를 선택합니다.  
> .prev(): 이전 형제 요소를 선택합니다.  
> .next(): 다음 형제 요소를 선택합니다.  
>> /jQuery/findParentChild.html  
>> /jQuery/findSiblings.html  

 ##### 문서 조작
> 클래스 조작
> .addClass(): 요소 내에 클래스를 추가합니다.  
> .removeClass(): 요소 내의 클래스를 제거합니다.  
> .toggleClass(): 요소 내의 클래스를 번갈아 가며 추가 또는 삭제(토글)합니다.  
> /jQuery/classControl.html  


> 속성 조작
> .attr(속성): 요소 내의 속성을 읽어 옵니다.  
> .attr(속성,값): 요소 내의 속성을 추가합니다.  
> .removeAttr(속성): 요소 내의 속성을 제거 합니다.  
> /jQuery/attributeControl.html  

> 스타일 조작
> .css(속성): css 속성을 읽어옵니다.  
> .css(속성,값): css 속성을 변경합니다.  
> /jQuery/styleControl.html  

> 문서 정보 조작
> .html(): 요소 내의 HTML을 읽어옵니다.  
> .html(값): 요소 내에 HTML을 추가합니다.  
> .text(): 요소 내의 텍스트 정보를 읽어옵니다.  
> .text(값): 요소 내에 텍스트 정보를 추가합니다.  
> /jQuery/documentControl.html  

> 문서 객체 추가
> .append(content): 지정한 선택자(요소) 안의 뒤에 추가합니다.  
> .prepend(content): 지정한 선택자(요소) 안의 앞에 추가합니다.  
> .after(content): 지정한 선택자(요소) 뒤(형제)에 추가합니다.  
> .before(content): 지정한 선택자(요소) 앞(형제)에 추가합니다.    
> /jQuery/addDocumentObject.html

> 문서 객체 이동
> .appendTo(요소명): 지정한 선택자(요소) 안의 뒤에 추가합니다.
> .prependTo(요소명): 지정한 선택자(요소) 안의 앞에 추가합니다.
> /jQuery/moveDocumentObject.html



 ##### jQuery 애니메이션
```
    .animate(속성, [재생 시간], [easing], [콜백 함수])

    속성: 애니메이션을 적용하려는 속성을 작성합니다.
    재생 시간: 애니메이션 재생시간을 ms 단위로 지정합니다.
    easing: 속도 변화 옵션을 적용합니다.
    콜백 함수: 애니메이션 재생이 끝난 후 처리할 콜백 함수를 지정합니다.
```
> /jQuery/animation.html

 ##### jQuery 이벤트
> 이벤트 타입 메서드  
> /jQuery/eventTypeMethod.html  
```
    $('문서 객체명').click(function(){
        // ...
    });
```

> on() 메서드  
> /jQuery/onMethod.html  
```
    $('문서 객체명').on('이벤트명', function(){
       // ...
    });
```


</p>
</details>






<details><summary>다이나믹 배너</summary>
<p>


</p>
</details>
