import random
from random import randint
game_level = print("1. easy 1-10 \n2. medium 1-20 \n3. hard 1-50\n4. quit")
gamer_choice = int(input('What level do you want to play (1),(2),(3), or (4)? '))
print()

def game1():
    guess_count = 0
    computer_guess = randint(1,10)
    while guess_count < 5:
        guess_count += 1
        gamer_guess = int(input("Choose a number 1 to 10"))
        if gamer_guess < computer_guess:
            print('Guess is too low')
        elif gamer_guess > computer_guess:
            print('Guess is too high')
        elif computer_guess == gamer_guess:
            print(' You won!')
    print('you lost all your chances')
print()
    
def game2():
    guess_count = 0
    computer_guess = randint(1,20)
    while guess_count < 5:
        guess_count += 1
        gamer_guess = int(input("Choose a number 1 to 20"))
        if gamer_guess < computer_guess:
            print("guess is too low")
        elif gamer_guess > computer_guess:
            print("guess is too high")
        elif computer_guess == gamer_guess:
            print('You won!')
    print('you lost all your chances')

def game3():
    guess_count = 0
    computer_guess = randint(1,50)
    while guess_count < 5:
        guess_count += 1
        gamer_guess = int(input("Choose a number 1 - 50"))
        if gamer_guess < computer_guess:
            print("guess is too low")
        elif gamer_guess > computer_guess:
            print("guess is too high")
        elif computer_guess == gamer_guess:
            print('You won')
    print('you lost all your chances')
    
print()

while gamer_choice != 4:
    if gamer_choice == 1:
        print(game1 ())
    elif gamer_choice ==2:
        print(game2())
    else:
        print(game3())
    gamer_choice = int(input('What level do you want to play (1),(2),(3), or (4)?'))
        
            
    
        
    
    

