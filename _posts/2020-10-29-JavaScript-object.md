---
title: 'JavaScript | Object 객체의 개념과 사용'

categories: TIL JavaScrtipt 기본 Object

tags: TIL JavaScript 기본 Object 

toc: true

date: 2020-10-29 14:19:28 -0400


---





# JavaScript | Object 객체의 개념과 사용





### <u>Object 객체의 개념 정리</u>

아마 자바스크립트를 배우기 시작하신 분들은 **'객체'**에 대해 들어보셨을 것이다.

이 글은 초심자, 혹은 어느 정도 객체를 들여다 본 분께 도움이 될 것 같다. 객체를 자유롭게 쓰고 수정하는 것이 아직은 어색한 분들께 이 글이 도움이 되었으면 좋겠다.



#### 들어가기 앞서.. 

자바스크립트의 거의 모든 것은  **객체**라고 생각하면 된다. 객체가 아닌 것들은 정해져있다. 바로 기본 데이터 타입인 boolean, number, string과 특별한 값인 null, undefined이다. 그 이외에 함수, 배열 등 자바스크립트의 요소는 다 객체이다.



#### 그렇다면 객체란 무엇일까?

일단 어렵게 생각하지 말고 **객체 = '{key: value}' 형태의 프로퍼티들을 저장하는 컨테이너**라고 생각하자.

![image-20201031222732799](/assets/image-20201031222732799.png)

간단한 객체를 가지고 왔다. 

여기서 키는? car, animal, color이고 밸류는? pontiac, Egytian vulture, green이다. 그렇다면 아래의 사진을 보자. 잘 정리된 상자 이미지에 각각의 키와 밸류를 넣어 이해해보자.



 ![img](/Users/edieko/coding/positiveko.github.io/_posts/2020-10-29-JavaScript-object.assets/image.png)![img](/Users/edieko/coding/positiveko.github.io/_posts/2020-10-29-JavaScript-object.assets/1553325719350_e5724b53410a3ea28d2a3e01f93d4fba.pn)

파일철을 담고 있는 박스는 곧 **Data**이다. 그리고 그 Data 안에는 3개의 파일이 있다. 이 파일이 바로 **key**이다. car, animal, color 라는 이름의 파일이 컨테이너 안에 들어가 있다. 그리고 그 안에는 여러 **value**들이 있을 것이다. 

객체는 왜 좋은 것인지 이 그림으로 알 수 있다.

우리는 이 잘 정리된 객체를 통해 수없이 **다양한 value들을 key를 인덱스 삼아 빠르고 정확하게 찾을 수 있을 것**이다. 당신이 객체를 잘 쓸 수 있다면, 빠르고 수월하게 자료들을 다룰 수 있을 것이다. 





### <u>Object 객체 읽고 쓰고 수정하기</u>

그렇다면 어떻게 객체를 이용할 수 있을까?

먼저 객체를 만들어 보자. 

#### 1) 객체 쓰기

![image-20201101132928147](/Users/edieko/coding/positiveko.github.io/_posts/image-20201101132928147.png)

먼저 Data를 {} 중괄호로 선언해주었다. 객체라는 뜻이다. 
이 빈 객체에 각각의 key를 . 온점을 찍어 표현하고 : 콜론 뒤에 ''value''를 적어주었다. 



#### 2) 객체 읽기 

만들어진 객체의 value값을 불러올 때에는 온점(.)과 대괄호[] 를 사용한다.

**온점.** 객체를 만들 때와 마찬가지로 온점을 찍어 value를 불러올 수 있다. 

![image-20201031224749956](/Users/edieko/coding/positiveko.github.io/_posts/image-20201031224749956.png)

혹은 **대괄호[]**를 적어서 불러올 수 있다. 주의점은 반드시 따옴표를 넣어주어야 한다!

![image-20201101140110470](/Users/edieko/coding/positiveko.github.io/_posts/2020-10-29-JavaScript-object.assets/image-20201101140110470.png)

온점을 사용하는 것이 더 편할 것 같은데 그렇다면 언제 대괄호를 사용할까?

✧ **스페이스가 포함된 키**는 반드시 대괄호로 접근해야 한다. (eg. Data['my name'])
✧ **숫자로 된 키**는 대괄호로 접근해야 한다. (eg. Data['3'])







#### 3) 객체에 키와 밸류 추가하기

객체에 값을 더 추가해보자.

배열은 추가할 수 있을까? 객체는 추가할 수 있을까? 가능하다.

![image-20201101133515326](/Users/edieko/coding/positiveko.github.io/_posts/image-20201101133515326.png)

만들어진 Data에 array 키를 만들어 배열을 넣어주었다. 
그리고 객체를 넣기 위해 person이라는 키를 객체로 선언해주었고, 다시 person에 키와 밸류를 넣어주었다. 

<u>다만 주의할 점은, Data.person이라는 키를 객체로 선언하지 않고 바로 Data.person.name을 만들 수는 없다. 객체로 먼저 선언을 해주자.</u>



#### 4) 객체의 모든 키와 밸류를 불러오기

객체를 읽을 때 한 번에 처리하고 싶다면 for in을 사용하자.

![image-20201031230718256](/Users/edieko/coding/positiveko.github.io/_posts/2020-10-29-JavaScript-object.assets/image-20201031230718256.png)

이렇게 한 번에 key와 value를 불러올 수 있다.



#### 5) 객체 관련 메소드

혹은 Object 관련 메소드를 사용할 수 있다.

![image-20201101134822506](/Users/edieko/coding/positiveko.github.io/_posts/image-20201101134822506.png)

**1) Object.keys()**

​	해당 객체 메소드는 인자로 전달된 객체의 모든 키들을 배열로 보여준다. 우측 콘솔창에 키로 이뤄진 배열이 만들어진 것을 알 수 있다.

**2) Object.values()**

​	이 메소드는 밸류들을 배열로 보여준다. 마찬가지로 values로 이뤄진 배열을 볼 수 있다.

**3) Object.assign(target, source)**

​	이 메소드는 인자로 받은 객체들을 합쳐준다. 위의 newData에 Data와 DataCopy의 키와 밸류들이 그대로 들어간 것을 볼 수 있다. 객체를 3개 이상 넣어줘도 다 합쳐준다. 혹은 source를 쓰지 않고 target만 써준다면 target을 그대로 클로닝 해준다. (마치 배열 메소드의 slice() 처럼!)



#### 6) 객체는 레퍼런스로 저장된다 

![image-20201101141527249](/Users/edieko/coding/positiveko.github.io/_posts/image-20201101141527249.png)

객체를 비교할 수 있을까? 같은 키와 밸류를 각각 다른 변수명으로 저장했다. 
그 안에서 Data.color == Data.name은 같은 밸류를 갖고 있으므로 true이다.

다만 같은 키와 밸류를 담은 변수 자체를 비교하면 false가 나온다. 

그 이유는 변수에 객체 리터럴 자체를 저장하는 것이 아니라 객체가 담긴 어느 메모리의 reference를 저장하기 때문에 실제 Data와 DataCopy가 갖고 있는 진짜 값은 다른 것이다. 





