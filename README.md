# HTML
## 0. HTML과 Tags
태그는 HTML의 핵심이다.
통계에 따르면 사이트마다 평균적으로 26개 정도의 태그를 사용한다.
이 정도는 빠삭하게 익히도록 하자.  
https://velog.io/@peacepiece27/HTML-핵심정리
## 1. 단락 Tags
`<br>`로 개행을 할 수 있다.  
하지만 단락을 표현할때는 `<p></p>`를 이용해 그룹핑하는 것이 더 좋다.  
하지만 여기에도 단점이 있는데 단락간의 간격을 조절할 수 없기 때문이다.
### 1.1 CSS
`</p><p style="margin-top:45px;">`와 같은 형식으로 단락의 줄 간격을 표현할 수 있다. 이를 CSS 문법이라 한다.

## 2. 속성(attribute)
`<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png">`  
이 코드를 사용하면 문서에 이미지를 표시할수 있다.
### 2.1. src
이미지의 주소를 값으로 가지는 속성이다
### 2.2. width
이미지의 크기가 화면 너비의 몇 퍼센트인지를 값으로 가지는 속성  
`<img src = ~ width = "100%">`라면 이미지가 페이지의 좌우를 꽉 채운다.

## 3. 태그 간의 관계
`<parent>`  
`<child></child>`  
`</parent>`  
태그 안의 태그는 자식 태그  
밖에 있는 태그는 부모 태그
### 3.1. 리스트 태그
`<li></li>` 태그로 리스트를 표현할수 있다. 
`<ul></ul>` unordered list의 줄임말. 목차가 필요없는 list의 요소들을 묶는다고 생각하면 된다.
`<ol></ol>` ordered list의 줄임말. list에 번호를 매겨야하는 요소들을 묶는다.

## 4. Top 5 태그
### 4.1. 본문을 설명하는 태그
`<title> ~ </title>`   
탭에 표시되는 웹페이지의 이름을 설정할수 있는 태그  
`<meta charset = "utf-8>`  
인코딩 방식을 설명하는 태그  
이런 태그들은 `<head></head>`에 들어가게된다.
### 4.2. 본문 태그
`<body></body>`
본문은 이 태그 안으로 들어가게된다.

## 5. 하이퍼링크
`<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 specification">Hypertext Markup Language (HTML)</a>` <br><br>
`target = "_blank"`라면 새창에서 링크가 열린다.  
`href` 속성은 링크의 주소  
`title` 속성은 링크 위에 마우스를 올려놓았을때 표시되는 주소.

## 6. 부록
### 6.1. 동영상 삽입
`<iframe width="1600" height="900" src="https://www.youtube.com/embed/jSJM9iOiQ1g?autoplay=1&mute=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>`  
유튜브 동영상을 삽입하는 코드이다. 일부 속성들이 앞에서 배운 요소들과 겹치는 것을 알 수 있다. `src`는 경로, `title`은 커서를 올려놓았을때 설명이다. 이처럼 중복되는 속성이 많으니, 공통적으로 반복되는 속성은 외워두도록 하자.  
임베디드 주소 옆에 autoplay를 삽입하여 자동재생이 가능하게했다. *Google Chorme*에서는 mute=1 로 해주지 않으면 재생되지 않기에 이도 함께 설정했다.  
`<iframe></iframe>` 태그는 외부의 HTML 페이지를 표시하는 기능을 가졌다.
### 6.2. target 속성
목차를 기존의 코드에서 분리하게 되면서 target 속성을 변경해, 창이 뜨는 방법을 변경했다.
https://tcpschool.com/html-tag-attrs/a-target