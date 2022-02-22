- How to create Stateless,ful Widgets
```
stl + TAB
stf +TAB
```
- What is hot reload and hot refresh  
```
- Hot Reload : 앱의 State는 유지하되 Widget Tree만 재구성하고 main() 및 initState()는 다시 호출되지 않는다.
- Hot Restart : 앱을 새로 시작하며 기존의 State를 잃게 된다.
```
- How to use Containers to lay out your UI  
    Container는 가능한한 가장 큰 공간을 가지려하고, child가 생기면 해당 child에 맞게 크기가 정해진다.   SizedBox는 Container와 기능은 같지만 높이와 너비를 지정할 수 있는 위젯이다  
    패딩을 정할 때 TRBL을 지정할 수도 있고, 수평과 수직을 EdgeInsets.symmetric(horizontal: 10.0)로 설정 할 수도 있다

- How to use Columns and Rows to position your UI elements  
    mainAxisAlignment와 crossAxisAlignment를 통해 아이템을 정렬한다  
    
- How to add custom fonts  
    pubspec.yaml의 flutter하위요소로 font속성을 지정한다  
```dart
flutter:
  fonts:
  - family: Pacifico
    fonts:
    - asset: fonts/Pacifico-Regular.ttf

  - family: Source Sans Pro
    fonts:
    - asset: fonts/SourceSansPro-Regular.ttf
```
- How to add Material icons
```dart
Icon(
    Icons.email,
    color: Colors.teal,
)
```
- How to style Text widgets  
    최상단 MaterialApp에서 theme으로 전체적인 설정 가능  
    constants.dart 내에 특정 스타일을 const로 선언 후 사용 가능
```
Text(
    'ABC',
    style: TextStyle(
        color: Colors.teal.shade900,
        fontFamily: 'Source Sans Pro',
        fontSize: 20.0,
    ),
)
```