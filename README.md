## 실시간 모니터링 시스템을 만들며 정복하는 MEVN 

오탈자는 다음과 같습니다. 1쇄를 기반으로 표기 됩니다.  

10p

> before

참고 : slice란

> after

참고 : slice를 이용한 얕은 복사

31p

> before

 ^은 0.12.1부터 1.0 미만의 버전과 호환된다는 의미입니다. 
 

> after

^0.12.1은 0.12.1부터 1.0 미만의 버전과 호환된다는 의미입니다. 

72p

> before

 front나 enqueue 등 큐의 필수적인 메서드를 정의했습니다. 큐는… (생략)   

> after

가장 앞의 있는 요소를 참조하는 front나 뒤에서 요소를 더하는 enqueue 등 큐의 필수적인 메서드를 정의했습니다.

83p

> before

콘솔을 출력하는 로직입니다. 

> after

콘솔을 출력도 하는 로직입니다.

98p

> before

npm install vo nightmare를 통해 설치합니다. 

> after

npm install vo nightmare를 통해 설치합니다. 
nightmare의 경우 m1 맥북에서 설치가 안되는 이슈가 있습니다. npm install --arch=x64 nightmare 이렇게 설치하면 됩니다. 


131p

> before

참고 : slice란?

> after

참고 : slice를 이용한 얕은 복사

132p

> before

대체하는 것입니다.  

> after

대체하는 원리입니다.  

136p

> before

console.log(a_lazy())

> after

const a_lazy = a(12010)
console.log(a_lazy())

143p

> before

모나드는 컨텍스트 레벨을 값 레벨로 끌어들여 추상화한 컨테이너박스를 말합니다. 개념적으로는 .. (생략)

> after

모나드는 컨텍스트 레벨을 값 레벨로 끌어들여 추상화한 컨테이너박스이자 카테고리 이론에서 사용되는… 

146p

> before

클로저란 외부함수의 실행 컨텍스트가 소멸해도 [[scope]] 프로퍼티가 가리키는 외부함 수의 실행환경이 소멸하지 않고 참조할 수 있는 것을 말합니다. 스코프체인이 형성될 때 [[scope]]로 참조할 수 있는데, 이를 이용해 참조할 수 있는 것을 말합니다. 잘 이해되지 않 는다면 뒷 장에 나오는 설명한 ‘자바스크립트의 실행 컨텍스트’ 글상자를 참고하세요. 
클로저의 예는 다음과 같습니다. 

> after

클로저란 외부함수의 실행 컨텍스트가 소멸해도 [[scope]] 프로퍼티가 가리키는 외부함수의 실행환경을 참조할 수 있는 것을 말합니다. 스코프체인을 형성할 때 [[scope]] 프로퍼티로 선언된 것을 이용한 것이죠. 클로저의 예는 다음과 같습니다.

147p

> before

앞의 코드는 count라는 private 변수를 만듭니다. test라는 함수는 getValue를 통해서만 count가 어떤 값인지 확인할 수 있습니다. 

> after

앞의 코드는 count 변수를 private 변수로 만들어 getValue 함수를 통해서만 count가 어떤 값인지를 확인할 수 있게 했습니다.

148p

 > before 

함수의 스코프 주소를 차례로 담은 리스트입니다. 순차적으로 탐색하며 해당 주소, 즉 [[scope]]로 참조가 가능합니다. 현재 실행 컨텍스트의 활성 객체(AO, Activation Object)를 선두로 하여 순차적으로 상위 컨텍스트의 활성 객체를 가리 키며 마지막 리스트는 전역객체(GO, Global Object)를 가리킵니다. 이때 AO나 GO 모두는 아직 값이 정해지지 않았고 빈 껍데기인 상태입니다. 좀 더 자세히 말하 면, 자신의 실행환경, 자신을 포함하는 외부 실행환경, 전역객체를 순차적으로 가리 키며 리스트를 만들게 됩니다. 이렇게 변수를 찾는 과정을 스코프체이닝이라고 합 니다. 이 스코프체인이 형성될 때 [[scope]]로 참조할 수 있는데, 이를 이용해 참조 할 수 있는 것을 클로저라고 합니다. 

 > after

함수의 스코프 주소를 담은 리스트를 스코프체인이라고 합니다. 현재 실행 컨텍스트의 활성 객체AO(Activation Object)를 선두로 하여 순차적으로 상위 컨텍스트의 활성 객체를 가리키며 마지막 요소는 전역객체GO(Global Object)가 들어갑니다. 이때 AO나 GO 모두 값이 정해지지 않은 빈 껍데기인 상태입니다. 참고로 이렇게 형성된 스코프체인의 [[scope]]를 통해 변수를 찾아가는 과정을 스코프체이닝이라고 합니다.  

166p

 > before 

보통 화면에서 6개 정도를 설정하는 것이  

 > after

보통 화면에서 30개 이하로 설정하는 것이  

172p


 > before 

하지만 DOM 트리와 렌더트리는 1:1
대응이 됩니다


 > after
 
하지만 DOM 트리와 렌더객체는 1:1
대응이 됩니다


252p

 > before 

모델이 가지고 있는 정보를 따로 저장해서는 된다.

 > after
 
모델이 가지고 있는 정보를 따로 저장해서는 안된다.

252p

 > before 

2. 모델이나 컨트롤러와 같이 다른 구성요소들을 몰라야 한다.  

 > after

2. 모델이나 뷰모델과 같이 다른 구성요소들을 몰라야 한다.  


328p

 > before 

MongoDB의 각 도큐먼트는 _id라는

 > after

MongoDB의 각 도큐먼트는 ObjectId라 불리는







