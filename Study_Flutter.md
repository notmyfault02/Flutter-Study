# Flutter를 공부하며 쓰는 내용

* 모든 개체들은 Widget으로 구성됨

~~~
return Scaffold(
  appBar: AppBar(
      title: Text(텍스트)
  ),
  body: Center(

  ),
  floatingActionButton: FloatingActionButton(
      onPressed: 동작
  ),
); //Scaffold 구조

~~~

* Container는 xml의 view같은 느낌, 화면 디자인할 때, 여백을 Container로 사용함

## 자주 나오는 문법
* @required: 객체나 라이브러리를 가져와서 쓸 수 있게 해줌(input과 비슷한 개념)
* <> (제네릭): 타입을 지정해 줌, 제네릭에 대한 내용은 더 자세하게 공부할 예정
* 식별자가 _(underline)로 시작하면 private로 선언됨. public이나 private를 사용할 필요 없음

## JSON 알아가기

### JSON 문법

~~~
{
  "userId" : 1,
  "id" : 1,
  "title" : "title"
  "body" : "body"
  "member": [
    {
      "name": "name",
      "age": 39
    }
  ]
}
~~~
* 문자열은 쌍따옴표로 묶어줌, 주로 중괄호, 대괄호 사용
* "설명하고자 하는 바" : "내용"
* @JSONSerializations: JSON을 직렬화한다, fromJSON()과 비슷한 느낌

### toJSON(), fromJSON() 차이
* toJSON(): 객체->JSON으로
* fromJSON(): JSON -> 객체로

### Todo 앱 만들기(3/6 ~)
* 참고: https://github.com/sabinbajracharya/fluttery-todo 
* Colorpicker 패키지 사용

## 3/9
* 내용 추가 액티비티 수정
* 내용 액티비티 색상 수정 시 메인 AppBar 색상 수정기능 개발중