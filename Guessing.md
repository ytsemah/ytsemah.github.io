
```mermaid
flowchart TD
Start([Start]) --> X[/Computer generates a random number/]
X --> B(Guess a number)
B --> C{{Is the input a number?}}
C --> D>The input is not a number]
D --> B
C --> E>The input is a valid number]
E --> F{Is the guess correct?}
F --> G>No, the guess is too high]
F --> H>No, the guess is too low]
G --> I((Try again!))
H --> I
I -.-> B
F --> J>Yes, the guess is correct]
J --> K(Go again?)
K --> L{{Yes}}
L -.-> X
K --> M{{No}}
M --> End([End])
```
#### The program starts, and a random number is generated.
#### The user is prompted to guess a number.
#### If the input is a valid number, the code continues. If not, they are prompted to input a number again.
#### If the number inputted is not equal to the randomly generated number, the user is told if they guessed higher or lower than the actual number and are then prompted to guess again.
#### If the number inputted is equal to the randomly generated number, the user is asked if they want to play again.
#### If the user wants to play again, the process repeats and a new random number is generated.
#### If the user does not want to play again, the code ends.

