# Python-Guessing_game
Guess a number between 1&amp;50 the program will message everything you need to know


#Number guessing game
#Liviu Silaghi
#02/11/2020

print('Welcome to my guessing game program')
input("\nReady? press Enter to begin")

import random


number = random.randrange(1,50)
guess = int(input('Guess a number between 1 and 50:'))
score=0
while guess != number:
    if guess < number:
        print('You need to go higher')
        guess = int(input('\nGuess a number between 1 and 50:'))
        score=score+1
    else:
        print('You need to go lower')
        guess = int(input('\nGuess a number between 1 and 50:'))
        score=score+1

print('You guessed correctly number of attempts',score)

input("\nWell done - press Enter to exit")
