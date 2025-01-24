# Random Number Guessing Game!

```mermaid
flowchart TD
  Start([Start]) --> A[Generate a Random Number]
  A --> B[Player makes a guess]

  B --> |Valid numeric input| Compare[Check Guess]
  B --> |Invalid input| Error[Invalid Input. Please Try Again.]
  Error --> B

  Compare --> |If the Guess is _**less then**_ the Random Number| Low[Too Low!]
  Compare --> |If the Guess is _**greater then**_ the Random Number| High[Too High!]
  Compare --> |If the Guess is _**equal**_ to the Random Number| Win[Congratulations! You have correctly guessed the number!]

  Low --> B
  High --> B
  Correct --> End([End])
```

#### This is my Number Guessing Game that I created where the player makes a guess. The computer will first generate a number which the player will be trying to guess. Once created, it will first check if the numeric input is valid or not. If it's valid, the flowchart continues. If the numeric input is invalid, the player will be asked to try again. If the player's guess is less then the random number, a "Too Low!" will be displayed. If the player's guess is greater then the random number, a "Too High!" will be displayed. Once the player guesses the correct number, a "Congratulations! You have correctly guessed the number!" will be displayed.
