'''mermaid

flowchart TD

Start([Start]) -->

Main --> Integer-SecretNumber;

Integer-SecretNumber --> Integer-UserGuess;

Integer-UserGuess --> IntegerMAX;

IntegerMAX --> MAX-equals-8;

MAX-equals-8 --> SecretNumber-equals-Random-MAX;

SecretNumber-equals-Random-MAX --> Output-**_Please-enter-a-number-between-0-and-&-MAX-1_**;

Output-**_Please-enter-a-number-between-0-and-&-MAX-1_** --> Input-UserGuess;


Input-UserGuess --> UserGuess-GreaterThan-LessThan-SecretNumber;

UserGuess-GreaterThan-LessThan-SecretNumber --> UserGuess-LessThan-SecretNumber;

UserGuess-LessThan-SecretNumber --> Output-**_Too-Low_**;

Output-**_Too-Low_** --> Output-**_Please-enter-a-number-between-0-and-7_**;

Output-**_Please-enter-a-number-between-0-and-7_**--> Input-UserGuess



Input-UserGuess --> UserGuess-GreaterThan-LessThan-SecretNumber;

UserGuess-GreaterThan-LessThan-SecretNumber --> UserGuess-GreaterThan-SecretNumber;

 UserGuess-GreaterThan-SecretNumber --> Output-**_Too-High_**;

Output-**_Too-High_** --> Output-**_Please-enter-a-number-between-0-and-7_**;

Output-**_Please-enter-a-number-between-0-and-7_** --> Input-UserGuess;


Input-UserGuess --> User-equals-SecretNumber;
User-equals-SecretNumber --> Output-**_Correct!_**;

Output-**_Correct!_** -->End([End])

'''
