# Guessing Game FlowChart

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

## Description of each step of the process.
### Part 1: Declare Section
> Function Main

> Declare Integer SecretNumber

> Declare Integer UserGuess

> Declare Integer MAX


### Part 2: Assign/In and Output Section
 > Assign MAX = 8

>  Assign SecretNumber = Random(MAX)
    
  > Output "Please enter a number between 0 and " & MAX - 1
  
   > Input UserGuess
    
> While UserGuess <> SecretNumber
    
 > If UserGuess < SecretNumber
     
  > Output "Too Low"
     
   > Else
      
  > If UserGuess > SecretNumber
     
  > Output "Too High"
      
   > End
       
   > End
     
 > Output "Please enter a number between 0 and 7"
     
  > Input UserGuess
     
 > End
    
> Output "You are Correct!"
    
End

