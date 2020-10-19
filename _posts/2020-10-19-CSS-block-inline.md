---

title: 'CSS 기본 01 - Block vs Inline vs Inline-block'

categories: TIL CSS 기본

tags: TIL Block Inline CSS

toc: true

---


# CSS 기본 01 - Block vs Inline vs Inline-block


안녕하세요, 오늘은 CSS의 기본!  
Display 프로퍼티 중에서도 inline, block, inline-block에 대해 알아보도록 하겠습니다.  
  

## inline  
inline에 속하는 html 태그에는 ```<span> <a> <img> <input> <label> <button> ```
inline으로 작성하면 줄 바꿈이 되지 않고 width와 height를 지정할 수 없습니다. inline 요소는 주로 글자에 하이라이팅 효과를 넣거나 문장에 효과를 주기 위해 사용합니다. 

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



## block
block에 속하는 html태그는 ```<div> <p> <header> <form> <h1> <table>``` 등이 있습니다.  
줄 바꿈이 되는 태그로 박스와 같은 형태를 띄기 때문에 문단을 표시하는 데 쓰일 수 있습니다. height와 width를 정할 수 있tmqslek.  


## inline-block
block과 inline의 중간 형태로 줄 바꿈이 되지 않지만 크기를 지정할 수 있습니다. 
