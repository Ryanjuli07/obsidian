```dart
void main() {
  // 1. Operator
  int a = 10;
  int b = 5;
  int sum = a + b; // Penjumlahan
  int product = a * b; // Perkalian
  bool isGreater = a > b; // Operator perbandingan
  
  print('Sum: $sum');
  print('Product: $product');
  print('Is a greater than b? $isGreater');

  // 2. Map
  Map<String, int> studentScores = {
    'Rehan': 90,
    'Askia': 85,
    'Rul': 88
  };

  // 3. List
  List<String> students = ['Rehan', 'Askia', 'Rul'];

  // 4. Set
  Set<String> uniqueStudents = {'Rehan', 'Askia', 'Rul', 'Rehan'}; // Set otomatis menghilangkan duplikat

  // 5. Simbol
  Symbol sym = #studentScores;
  print('Symbol: $sym');

  // 6. Percabangan
  String getGrade(int score) {
    if (score >= 90) return 'A';
    if (score >= 80) return 'B';
    if (score >= 70) return 'C';
    return 'D';
  }

  // 7. Perulangan
  for (var student in students) {
    print('$student has grade ${getGrade(studentScores[student]!)}');
  }

  // 8. Function parameter and optional parameter
  String greet(String name, [String greeting = 'Hello']) {
    return '$greeting, $name!';
  }

  print(greet('Rehan')); // Greeting default
  print(greet('Askia', 'Hi')); // Greeting custom

  // 9. Inner function
  int outerFunction(int x) {
    int innerFunction(int y) {
      return x + y;
    }
    return innerFunction(5);
  }

  print('Outer function result: ${outerFunction(10)}');

  // 10. Function return value
  int multiply(int x, int y) {
    return x * y;
  }

  // 11. Short expression
  int square(int x) => x * x;

  print('Product: ${multiply(3, 4)}');
  print('Square: ${square(5)}');

  // 12. Anonymous function
  List<int> numbers = [1, 2, 3, 4];
  numbers.forEach((number) => print('Number: $number'));

  // 13. Scope and closure
  Function makeCounter() {
    int count = 0;
    return () {
      count++;
      return count;
    };
  }

  var counter = makeCounter();
  print('Counter: ${counter()}');
  print('Counter: ${counter()}');
}
```