***mermaid
flowchart TD
    Start[Start] --> A[Set range for guessing: low=1, high=100]
    A --> B[Generate random number between low and high]
    B --> C[Initialize guessCount = 0]
    C --> D[Prompt user to imput a guess]
    D --> E{Is the user's guess correct?}

    E -- Yes --> F[Your guess is correct!]
    F --> G[Display total guesses made]
    G --> End([End])

    E -- No --> H{Is the guess too high?}
    H -- Yes --> I[Your guess is too high]
    I --> J[Increment guessCount]
    J --> D

    H -- No --> K{Is the guess too low?}
    K -- Yes --> L[Your guess is too low]
    L --> J

    K -- No --> D
***  
