import random

shaina = random.randint(1,100)
turn = 1

name = input("What is your superhero name? ")

while True:
    print(name + ", this is turn",turn)
    turn += 1

    player = int(input("Pick a number from 1-100 "))

    if shaina == player:
        print("You guessed it!")
        break
    elif shaina > player:
        print("Higher")
    else:
        print("Lower")  

    if turn == 8:
        print("You ran out of turns!")
        break      

print("Game over!")
