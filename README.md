# New_Project
#This is my first project uploaded to github!
#Its a guessing number game. enjoy!

import random

secretNum = random.randint(1,101)
print("I am thinking of a number between 1 and 100!")

#Ask the player to guess 6 times!
for guessTaken in range(1,7):
    print('take a guess: ')
    guess = int(input())

    if guess < secretNum:
        print('Your guess is too low')
    elif guess > secretNum:
        print('Your guess is too high')
    else:
        break #This condition is the correct input

if guess == secretNum:
    print("YOU GOT IT CORRECT!! It took you " + str(guessTaken) + " guesses!")
else:
    print("Nope, the number i was thinking of was " + str(secretNum))
    

input("Would you like to play again?: ")
