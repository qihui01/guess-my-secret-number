# guess-my-secret-number
Guess my secret number between 1 to 100
import random
    
num = random.randint(1, 100)
guess = None
    
while guess != num:
    guess = input("guess a number between 1 and 010: ")
    guess = int(guess)
    
    if guess == num:
        print("congratulations! you won!")
        break
    else:
        print("nope, sorry. try again!")
