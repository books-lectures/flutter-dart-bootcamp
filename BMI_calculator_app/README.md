- How to use Flutter themes to create coherent branding.
```dart
// copyWith를 통해 ThemeData의 일부값만 수정해 사용할 수 있다

return MaterialApp(
      theme: ThemeData.dark().copyWith(
        primaryColor: Color(0xFF0A0E21),
        scaffoldBackgroundColor: Color(0xFF0A0E21),
      ),
      home: InputPage(),
    );
```
- How to create multi-page apps using Flutter Routes and Navigator.
```dart
Navigator.push(
    context,
    MaterialPageRoute(
        builder: (context) => NextPage(),
    ),
);
```
- How to extract and refactor Flutter Widgets with a click of the button.  
    커스텀위젯을 만들기 위해서 가급적 RAW한, 저수준의 위젯을 골라야 한다  
    버튼에 있어 낮은 수준을 제공하는 위젯은 RawMaterialButton이 있다
```dart
RawMaterialButton(
    child: this.icon,
    onPressed: this.onPressed,
    shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(15.0)),
    elevation: 0.0,
    fillColor: Colors.redAccent,
    constraints: BoxConstraints.tightFor(
    width: 56.0,
    height: 56.0,
    ),
);
```
- How to pass functions as parameters and fields.
```dart
// 다트는 객체 지향 프로그래밍과 함수형 프로그래밍의 특징을 모두 제공한다  
// 함수형 프로그래밍은 자료 처리를 수학적 함수의 계산으로 취급하는 프로그래밍 패러다임이다 (상태와 가변 데이터를 기피한다)  

// 일급 객체
// 다트에서는 함수를 값으로 취급할 수 있다. 그러므로 다른 변수에 함수를 대입할 수 있다.
// 다른 함수의 인수로 함수 자체를 전달하거나 함수를 반환받을 수도 있다.
```

- How to use the GestureDetector Widget to detect more than just a tap.  
    onTap, onDoubleTap, onLongPress 등 다양한 이벤트들을 감지한다
- How to use custom colour palettes by using hex codes.
```dart
// HEX값 앞에 `0xFF` 추가

Color(0xFF0A0E21)
```
- Understand Dart Enums and the Ternary Operator.
```dart
// enums
enum Gender {
  male,
  female,
}

// Ternary Operator
colour: selectedGender == Gender.male
    ? kActiveCardColour
    : kInactiveCardColour,
```
