- How to incorporate open source libraries of code into your project using - Flutter Packages.  
**pub.dev** 에서 원하는 패키지 검색후 pubspec.yaml에 추가  
`flutter pub get`
- How to play sound on both iOS and Android.  
```dart
// audioplayers: ^0.17.4
// assets 파일내의 .wav파일을 재생한다
void playSound(int soundNumber) {
    final player = AudioCache();
    player.play('note$soundNumber.wav');
}
```
- How to generate repeated user interface Widgets.  
    flutter outlined에서 해당 위젯을 extract widget을 통해 추출한 후, 속성값을 생성자로 받아 다양한 위젯으로 재활용 한다

- What is the difference between var, const and final in Dart.  
### var
어떤 변수형도 담을 수 있지만 한번 설정되면 변경불가
```dart
var boo = 123;
boo = 'abc'; // Error
boo = 500; // OK
```
### dynamic
어떤 변수형도 담을 수 있고, 변경이 가능하다
```dart
dynamic boo = 123;
boo = 'abc'; // OK
boo = 500; // OK
```
### final 
최초 선언시 어떠한 변수형도 담을 수 있지만 선언 이후 변경 불가
```dart
final boo = 123;
boo = 567; // Error
boo = 'abc'; // Error
```
### const
최초 선언시 어떠한 변수형도 담을 수 있지만 선언 이후 변경 불가
```dart
const boo = 123;
boo = 567; // Error
boo = 'abc'; // Error
```
### var vs. dynamic
var은 최초에 담긴 변수형이 고정되고, dynamic은 변수형도 유동적이다
### final vs. const
const: 컴파일 타임에서 상수를 정의, 런타임에서 정의되는 값을 설정 불가
final: 런타임에서 결정되는 값(상수, 변수) 설정 가능
```dart
const DateTime now = DateTime.now(); // compile error
final DateTime now = DateTime.now(); // OK
```