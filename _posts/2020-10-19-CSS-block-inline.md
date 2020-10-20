---

title: 'CSS 기본 01 - Block vs Inline vs Inline-block'

categories: TIL CSS 기본

tags: TIL Block Inline CSS

date: 2020-10-19 18:19:28 -0400

toc: true

---




# CSS 기본 01 - Block vs Inline vs Inline-block

안녕하세요, 오늘은 CSS의 기본!  
Display 프로퍼티 중에서도 inline, block, inline-block에 대해 알아보도록 하겠습니다.  

![css display values](http://www.danielledeveloper.com/wp-content/uploads/2018/05/display-values-e1527791468578.png)






## inline  
inline에 속하는 html 태그에는 ```<span> <a> <img> <input> <label> <button> ```
inline으로 작성하면 줄 바꿈이 되지 않고 width와 height를 지정할 수 없습니다. inline 요소는 주로 글자에 하이라이팅 효과를 넣거나 문장에 효과를 주기 위해 사용합니다. 

다만, line-height 프로퍼티를 이용하면 height의 크기 조절이 가능합니다. 그리고 라인의 사이에는 기본적인 padding이 추가된다는 것을 주의해야 합니다.

```
<style>
.bold {
    font-weight: bold;
}
.underline {
    border-bottom: 1px solid black;
}
</style>

<p>
    Lorem ipsum dolor sit amet, <span class="bold">consectetur adipiscing elit</span>,
	sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
	Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
	Duis aute irure dolor in <span class="underline">reprehenderit</span>
	in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
	Excepteur sint occaecat cupidatat non proident,
	sunt in culpa qui officia deserunt mollit anim id est laborum.
</p>
```

![스크린샷 2020-10-20 오후 3.53.46](/Users/edieko/Desktop/스크린샷 2020-10-20 오후 3.53.46.png)

문단 사이에 <span>을 활용해서 밑줄을 긋거나 볼드체로 수정하는 등의 강조 표시를 넣을 수 있습니다. 





## block
block에 속하는 html태그는 ```<div> <p> <header> <form> <h1> <table>``` 등이 있습니다.  
줄 바꿈이 되는 태그로 박스와 같은 형태를 띄기 때문에 문단을 표시하는 데 쓰일 수 있습니다. height와 width를 정할 수 있습니다.

```html
<p>The following div is an <div class="highlight">block-level element;</div>
its background has been colored to display both the beginning and end of
the block-level element's influence.</p>
```

![스크린샷 2020-10-20 오후 3.56.20](/Users/edieko/Desktop/스크린샷 2020-10-20 오후 3.56.20.png)






## inline-block
block과 inline의 중간 형태로 inline 처럼 한 줄에 나타낼 수 있으면서도 block처럼 width와 height를 수정할 수 있습니다.

![Display: inline VS inline block. display:inline makes the element create… |  by nana Jeon | Design & Code Repository | Medium](https://cdn-images-1.medium.com/fit/t/1600/480/1*CmQvo3uVuSpjYkylaq-M2g.png)







참고 페이지

------

연습 페이지: https://codepen.io/nana8/pen/wrBBbw

참고 자료 http://www.danielledeveloper.com/inline-vs-block-vs-inline-block-css/

https://medium.com/design-code-repository/display-inline-vs-inline-block-fc6cbe6dc2bf