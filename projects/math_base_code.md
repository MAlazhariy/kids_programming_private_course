```dart
import 'dart:math';

int getRandomNumber(int min, int max) {
  return Random().nextInt(max - min) + min;
}


void showScore(int score) {
  print("Your Score is $score 🎉");
  print("----------");
}

// todo: Ask question function
// this function do:
// 1. Generate two nubmers from getRandomNumber function
// 2. show the question to the user and get the answer from the user
// 3. calculate the result & set is correct answer boolean
// 4. set the mark for the question if the answer is correct & show a message to the user
// 5. the function is int and returns the mark

void main() {
  int score = 0;
  int counter = 1;

  // todo: convert to (for)
  while (counter <= 5) {
    score += askQuestion();
    showScore(score);
    counter++;
  }
}
```
