'''Mermaid  
flowchart TD

    Start[Start] --> A[Set range for guessing: low=1, high=100]
    This will be the parameters of my game.
    A --> B[Generate random number between low and high]
    THis will be the number that the player will have to guess.
    B --> C[Initialize guessCount = 0]
    This is guess count as it starts at 0.
    C --> D[Prompt user to imput a guess]
    THe user will have to imput their number.
    D --> E{Is the user's guess correct?}
    It will have to compare the number imputed vs the number that was chosen.

    E -- Yes --> F[Your guess is correct!]
    THe user got the number right and is congratulated. 
    F --> G[Display total guesses made]
    Shows the number of tries it took the user.
    G --> End([End])

    E -- No --> H{Is the guess too high?}
    Will be able to tell if the number imputted is higher than chosen number.
    H -- Yes --> I[Your guess is too high]
    Displays that to user.
    I --> J[Increment guessCount]
    Shows the numebr of incorrect guesses.
    J --> D
    Takes user back to imput guess.

    H -- No --> K{Is the guess too low?}
    Will be able to tell if the number imputted is lower than the chosen number 
    K -- Yes --> L[Your guess is too low]
    Will inform the user that the number is lower.
    L --> D
    Takes user back to the imput prompt
'''
