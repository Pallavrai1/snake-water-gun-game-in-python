#snake water gun code in python
import random
print("Welcome to SWG game:")
player1 = 0
computer=0
for i in range(6):
    player1input = int(input("Enter your choices from 2,1,0 for snake,water,gun::"))
    x = [2,1,0]
    computerinput = random.choice(x)
    if(player1input==computerinput):
        print("match drawn")
        
        print("player1points",player1)
        print("computerpoints",computer)
    elif(player1input==2and computerinput!=0):
        print("you won")
        player1+=1
        print("player1points",player1)
        print("computerpoints",computer)
    elif(player1input==1and computerinput!=2):
        print("you won")
        player1+=1
        print("player1points",player1)
        print("computerpoints",computer)
    elif(player1input==0and computerinput!=1):
        print("you won")
        player1+=1
        print("player1points",player1)
        print("computerpoints",computer)
    else:
        print("you loose")
        computer+=1
        print("player1points",player1)
        print("computerpoints",computer)
    print("computerinput",computerinput)
if(player1>computer):
    print("player1 won")
else:
    print("computer won the game")
