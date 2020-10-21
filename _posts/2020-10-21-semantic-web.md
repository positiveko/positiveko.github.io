---
title: 'HTML 기본 01 Semantic Web, Semantic Tags'

categories: TIL HTML 기본

tags: TIL HTML semantic

toc: true

date: 2020-10-21 08:19:28 -0400

---

오늘은 Semantic Web과 Semantic Tags에 대해 알아봅니다.



# Semantic Web, Semantic Tags

> The Semantic Web is an extension of the current web in which information is given well-defined meaning, better enabling computers and people to work in coopertation. - Tim Berners-Lee.



Semantic Web이란 WWW을 만든 팀 버너스리가 제안한 차세대 웹 기술입니다. 웹 상에 존재하는 정보를 사람 뿐만 아니라 기계가 의미(semantic)를 파악하고 사용자의 요구에 적합한 결과를 서비스하도록 만들었습니다.

현재의 웹은 사용자가 목적에 맞게 정보를 찾는 방식이지만, 시맨틱 웹은 프로그램이 자동적으로 웹 상의 정보를 추출하고 가공하여 새로운 정보를 만들어냅니다. 이처럼 시맨틱 웹이 지향하는 목표는 1)웹 상의 정보들을 컴퓨터가 이해할 수 있는 형태의 언어로 바꾸는 것과 2)컴퓨터가 자동으로 방대한 정보들을 검색하고 이를 바탕으로 지식을 추론하는 것까지 발전하는 것이다. 





![현재의 웹에 온톨로지(지식자원의 의미정보 메타데이터)를 추가 구성하여, 컴퓨터가 온톨로지를 기반으로 스스로 추론하여 의미 있는 정보를 추출할 수 있도록 구성한 웹 시스템](http://www.frotoma.com/image/sub/company_5.png)



## Semantic Web 작동 방식

HTML의 요소는 non-semantic 요소, semantic 요소로 구분할 수 있습니다. non-semantic 요소에는 div, span 등이 들어가고, semantic 요소에는 form, img, table 등이 있습니다. 시맨틱 웹은 시맨틱 요소가 들어간 태그, 즉 시맨틱 태그를 기반으로 웹을 크롤링하게 됩니다. **Semantic Tag**는 브라우저, 검색 엔진, 개발자 모두에게 콘텐츠의 의미를 명확히 설명하는 역할을 합니다. 시맨틱 태그에 의해 컴퓨터가 HTML 요소의 의미를 보다 명확히 해석하고 그 데이터를 활용할 수 있는 시맨틱 웹이 실현될 수 있습니다. 

시맨틱 웹은 웹에 존재하는 수많은 웹페이지들에 메타데이터(Metadata)를 부여하여, 기존의 잡다한 데이터 집합이었던 웹페이지를 '의미'와 '관련성'을 가지는 거대한 데이터베이스로 구축합니다.



사이트에 이미지를 넣는 방식에는 img와 div로 background-image 속성을 추가하는 것 두 가지 방식이 있습니다. 둘의 차이점은 무엇일까요? semantic web의 작동 방식을 보았을 때  div로 넣는다면 웹이 자동으로 의미를 알 수 없기 때문에 단순히 웹 페이지의 장식 용도로 사용할 수 있습니다. 하지만 img 태그로 넣는다면 image를 담겠다는 뜻을 담기 때문에 semantic web이 그 이미지에 대한 정보를 크롤링할 수 있어 SEO(검색 엔진 최적화)에 맞는 페이지를 작성할 수 있습니다. 또한 'alt' attribution에 이미지에 대한 뜻도 담을 수 있습니다. 

따라서 본인이 만드는 페이지가 검색을 통해 검색 엔진에 뜨도록 하고 싶다면 최대한 semantic tag를 활용해서 작성하는 것이 맞습니다. 





참고자료

------

http://www.frotoma.com/sub2_1.do

https://poiemaweb.com/html5-semantic-web