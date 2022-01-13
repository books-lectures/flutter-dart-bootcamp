# flutter-dart-bootcamp
[The Complete 2021 Flutter Development Bootcamp with Dart] 강의 내용을 정리하는 레포지토리 입니다
<p align="center">
  <img src="https://user-images.githubusercontent.com/64571546/145810728-c9770647-08dc-4e73-9761-f51eac707fe7.png" />
</p>

20220112
클래스 내부에 const 변수를 만들려면 static 키워드를 사용해야 한다.
static 키워드는 클래스 공통 변수나 메소드이다.
공통 변수를 조회하기위해 불필요한 객체생성을 방지해준다.

20220113
mixin canSwim {
  void swim() {
    print('swiming')
  }
}

Class Fish extends Animal with canSwim, canFly {
  // mixin을 이용해 여러 클래스들의 기능을 가쟈올 수 있다
}

dart 코드리팩토링
중복되는 위젯은 flutter outline에서 extract widget을 통해 분리하고, 생성자를 통해 속성을 설정해 재사용한다

constants 속성들은 copywith()를 통해 바꾸고 싶은값만 바꿔서 
