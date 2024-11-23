# guess-my-secret-number
import random
    
num = random.randint(1, 100)
guess = None
guess_count = 0

while True:
    guess = int(input("Enter your guess between 1 and 100: "))
    guess_count += 1
    guess = int(guess)
    
    if guess == num:
        print("congratulations! you won!")
        break
    else:
        print("nope, sorry. try again!")

    if guess_count > 3:
        print("It's okay! The secret number is " + str(num))
        break 
