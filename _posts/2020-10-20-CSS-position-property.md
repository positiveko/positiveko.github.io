---
title: 'CSS 기본 02 - Position relative, absolute, fixed'

categories: TIL CSS 기본

tags: TIL position relative absolute fixed CSS

toc: true


---


# CSS 기본 02 - Position relative, absolute, fixed

안녕하세요, 오늘은 CSS의 기본!  
Position 프로퍼티 중에서도 relative, absolute, fixed에 대해 알아보겠습니다.

마지막에는 position property를 간단하게 연습할 수 있는 페이지가 있습니다. 
꼭 공부하고서 연습을 통해 개념을 이해합시다!




## Position property  

Position 프로퍼티는 문서 상에 요소를 배치하는 방법을 결정합니다. 
디폴트 값은 position: static으로 일반적인 문서의 흐름에 따라 요소가 배치됩니다. 

다음은 4개의 div에 display: inline-block을 주었습니다.

![Image for post](https://miro.medium.com/max/429/1*iVt-tUfGKHZyEkspuu7LlQ.png)



### position: relative

------

별도의 프로퍼티를 저장하지 않으면 static과 동일하게 배치됩니다. 
position: relative를 준 요소에 top, bottm, left, right 프로퍼티를 주면 기준이 되는 부모 요소 혹은 자신의 위치를 기준으로 하여 위치가 상대적으로 배치됩니다.

따라서 box two에 position을 relative로 주고 top: 20px, left: 20px를 주면 아래와 같이 기존의 위치에서 상대적으로 배치됩니다. 

![Image for post](https://miro.medium.com/max/455/1*3N2ousp3yth9ovHA8TpDZw.png)



### position: absolute

------

Position: absolute는 부모 요소를 기준으로 위치가 지정되어 고정됩니다. 
만약 부모 요소가 body라면 페이지 스크롤에 따라 움직입니다. 하지만 그 외의 경우에는 html에 대한 절대적인 위치로 고정됩니다.

absolute를 사용할 때 주의해야할 사항은 부모 요소의 position 프로퍼티가 static이 아닐 때(디폴트가 아닐 때)에는 부모 요소를 기준으로 위치가 결정된다는 것이다. 

![Image for post](https://miro.medium.com/max/343/1*XDqGjAEa_sNL1OlPQhEb7A.png)

### position: fixed

------

fixed는 위치가 지정되어 고정되는 것은 absolute와 같습니다. 
다만 부모 요소를 기준으로 위치가 고정되는 absolute에 반해 fixed는 뷰포트를 기준으로 위치를 고정합니다. 따라서 스크롤해서 창을 내리는 상황이라면 fixed는 위치가 고정되어 있겠지만, absolute는 부모 요소를 따라 웹페이지에서 이동할 것입니다.

아래에 있는 페이지에서 세 가지 프로퍼티를 적용해서 실습해봅시다! 









##### 참고 자료

------

아래의 페이지에서 position property 연습하기!

https://jsbin.com/nohoyiq/edit?html,css,output

이미지 출처

https://medium.com/@leannezhang/difference-between-css-position-absolute-versus-relative-35f064384c6

