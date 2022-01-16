# flutter-dart-bootcamp
[[The Complete 2021 Flutter Development Bootcamp with Dart] 강의](https://www.udemy.com/course/flutter-bootcamp-with-dart/) 내용을 정리하는 레포지토리 입니다
## Dart

## Section 1
- what is flutter?
- why flutter?
- flutter architectural overview
<img src="https://docs.flutter.dev/assets/images/docs/arch-overview/archdiagram.png" alt="Architectural
diagram" width="100%">
## Section 2
- Setup on mac
- Flutter with IntelliJ
## Section 3
- Add assets
- Generate app icon
## Section 4
- Setting for physical device
- Add another skin (galaxy20)
- Use various IOS simulator
## Section 5
- Useful sites
  - [Icons8](https://icons8.com/)
  - [Vecteezy](https://www.vecteezy.com/)
  - [Canva](https://www.canva.com/)
## Section 6
- Hot reload, hot restart
- Container widget
- Column, row widget
- Incorporate custom fonts
- [Flutter Layout Cheat Sheet](https://medium.com/flutter-community/flutter-layout-cheat-sheet-5363348d037e)
## Section 7
- Expanded class
- Flexible class
- Gesture detect class
## Section 8
- setState function
## Section 9
- Sound playing library
- [AudioCache Documentation](https://github.com/bluefireteam/audioplayers/blob/main/packages/audioplayers/doc/audio_cache.md)
## Section 10
- [Alert library](https://pub.dev/packages/rflutter_alert)
## Section 11
- Background image
## Section 12
- Use flutter themes
- Custom widget
- Flutter Slider class
- Route multiple screena
- Color with HEX code
- Font Awesome package
## Section 13
- Datas from platform(physical device)
- Statefull widget life cycle
- Networking with http package
- JSON parsing
- fromJSON, toMap object
- Spinner when user wait
## Section 14
- Dropdown widget
- Coupertino picker widget
- Platorm specific UI(Material, Cupertino)
## Section 15
- Hero Animation
- Curved Animation
- Firebase
   - Auth
   - Database
- Stream builder
## Section 16



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
