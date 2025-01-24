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
  Compare --> |If the Guess is _**equal**_ to the Random Number| Win[Congradulations! You have correctly guessed the number!]

  Low --> B
  High --> B
  Correct --> End([End])
```

#### This is my Number Guessing Game that I created where the player makes a guess. The computer will first generate a number which the player will be trying to guess. Once created, it will first check if the numeric input is valid or not. If it's valid, the flowchart continues. If the numeric input is invalid, the player will be asked to try again. 
