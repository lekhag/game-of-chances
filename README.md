# game-of-chances
import random
num = random.randint(1,10)
num1 = random.randint(1,10)
num2 = random.randint(1,10)

money = 100
coin =("Heads","Tails")
flip=random.choice(coin)
#Write your game of chance functions here

def coin_flip(bet,your_choice):
  if your_choice == flip:
    return "You have won "+ str(bet)
  else:
    return "you lost -" + str(bet)
#print(coin_flip(50,"Tails"))    

print(str(num1), str(num2))
def dices(bet,your_choice):   
  if your_choice == "even" and (num1+num2) % 2 == 0:
    return "you won " + str(bet)
  else:
    return "you lost -" + str(bet)
print(dices(20,"even"))

def deck(bet,num1,num2):
  if bet<= 0:
    return "you did not bet anything"
  elif num1 > num2:
    return "you won"
  elif num2 > num1:
    return "you lost"
  else:
    return "its a tie"
print(str(num1)+" " +str(num2))
print (deck(10,num1,num2))

