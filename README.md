# Learn C++ STL
### STL 공부 순서
1. STL에 대한 구조 공부
2. STL 구성요소 공부
3. STL를 이용한 예시 코드 작성


## STACK STL 공부
### 1. 스택이란?
* 스택은 컴퓨터에서 가장 많이 사용되는 자료 구조이다.
* LIFO : (Last-In-First-Out) 후입선출의 구조를 가진다.
![stack-gif](https://github.com/khs020512/LearnAPI/assets/97209803/bdb1f7bd-2cc3-4c5f-9230-bd4b6a7d661b)
### 2. 스택의 구성 요소
* **스택의 생성(선언) (Stack)**
  * 스택을 생성하는 연산
  * **stack<데이터 타입> 스택이름;** 의 형태로 생성한다
  ```
  stack<int> myStack;
  ```
* **스택 공백확인 연산 (empty)**

  * 스택이 비었는지 아닌지 확인하는 연산
  * Bool타입의 함수로 true 또는 false 로 return값이 생성된다.
  * **스택이름.empty()** 의 형태로 사용한다.
  ```
  if(!myStack.empty()){
    ...
  }
  ```
  
* **스택 크기 확인 연산 (size)**
  * 스택속의 데이터가 얼마나 들어있는지 확인하는 연산
  * int타입의 함수로 비었을 때에는 -1을 반환하고 비어있지 않을 때에는 크기 값을 반환한다
  * **스택이름.size()** 의 형태로 사용한다
  ```
  size = myStack.size();
  ```
* **스택 최상단값 확인 연산 (top)**
  * 스택의 최상단값을 확인하는 연산
  * 스택의 데이터 타입에 따라 반환하는 값이 다름
  * **스택이름.top()** 의 형태로 사용한다
  ```
  top = myStack.top();
  ```
* **스택 삽입 연산 (push)**
  * 스택속에 데이터를 삽입하는 연산
  * 스택의 최상단에 데이터를 저장함
  * **스택이름.push(데이터 값)** 의 형태로 사용한다
  ```
  myStack.push(10)
  ```
* **스택 삭제 연산 (pop)**
  * 스택속의 데이터를 삭제하는 연산
  * 스택의 최상단의 데이터를 삭제한다.
  *  **스택이름.pop()** 의 형태로 사용한다.
  ```
  data = myStack.pop();
  ```
* **스택 삽입 연산_2 (emplace)**
  * 스택의 push와 비슷한 연산
  * 특정 클래스의 스택일 경우 해당 args를 그 클래스의 생성자로넘겨 해당 클래스의 객체를 생성해 push한다.
  * **스택이름.emplace(args)** 의 형태로 사용한다.
  ```
  myStack.emplace("First sentence");
  ```
* **스택 바꾸기 연산 (swap)**
  * 두개의 스택을 바꾸는 연산
  * 서로 다른 스택이 있을 때 각 스택의 구성요소 전부를 서로 바꾼다.
  * **스택이름.swap(바꿀스택의 이름)** 의 형태로 사용한다.
  ```
  stack<int> foo.bar;
  ...
  foo.swap(bar);
  ...
  ```
## QUEUE STL 공부
### 1. 큐 란?
* 큐는 먼저들어온 데이터가 먼저나가는 **선입선출(First-In-First-Out)** 의 구조를 가진다.
! https://images.velog.io/images/godkor200/post/b31ed9db-aa01-4ac7-a3cd-0fd00295a65e/queue-gif.gif
### 2. 큐의 구성요소

## LIST STL 공부
