```mermaid
flowchart TD
    A[Start Game] -->|Generate Number between 1-100| B(Player inputs guess)
    B -->|Add 1 guess to total number of guesses| C{Compare player number with generated number}
    C -->|Too High| D[Guess again. Choose a lower number.]
    D -->B
    E -->G[End Game]
    C -->|Correct / Total Guesses Final| E[You Win!! Total Guess Counter: ]
    C -->|Too Low| F[Guess again. Choose a higher number.]
    F -->B
