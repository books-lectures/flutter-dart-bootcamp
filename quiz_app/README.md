- alert package  
```dart
// rflutter_alert: ^1.0.2

Alert(
    context: context,
    title: 'title!',
    desc: 'desc!',
).show();
```
- SafeArea()  
    충분한 패딩(들여쓰기)으로 자식(child)을 삽입하는 위젯
    SafeArea를 통해 노치나 카메라 영역에 상관없이 화면을 구성

- 클래스 내부에 데이터와 메소드를 활용해 데이터를 보여주는 예제
```dart
class QuizBrain {
  int _questionNumber = 0;

  List<Question> _questionBank = [
    Question('Some cats are actually allergic to humans', true),
    Question('You can lead a cow down stairs but not up stairs.', false),
    Question('Approximately one quarter of human bones are in the feet.', true),
    Question('A slug\'s blood is green.', true),
    Question('Buzz Aldrin\'s mother\'s maiden name was \"Moon\".', true),
    Question('It is illegal to pee in the Ocean in Portugal.', true),
  ];

  void nextQuestion() {
    if (_questionNumber < _questionBank.length - 1) {
      _questionNumber++;
    }
  }

  String getQuestionText() {
    return _questionBank[_questionNumber].questionText;
  }

  bool getCorrectAnswer() {
    return _questionBank[_questionNumber].questionAnswer;
  }

  bool isFinished() {
    if (_questionNumber >= _questionBank.length - 1) {

      print('Now returning true');
      return true;

    } else {
      return false;
    }
  }

  void reset() {
    _questionNumber = 0;
  }
}
```