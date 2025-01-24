# Random Number Guessing Game!

```mermaid
flowchart TD
  Start([Start]) --> A[Generate a Random Number]
  A --> B[User makes a guess]

  B --> |If Valid numeric input| Compare[Check Guess]
