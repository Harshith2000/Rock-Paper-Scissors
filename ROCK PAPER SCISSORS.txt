from random import randint
print("ROCK-R::SCISSORS-S::PAPER-R")
for i in range(100):
  player=input("R,S or P?")
  print(player,"vs",end=" ")
  gen=randint(0,2)
  if gen==0:
    opp="R"
  elif gen==1:
    opp="S"
  elif gen==2:
    opp="P"
  print(opp)
  if player==opp:
    print("DRAW!!")
  elif player=="R" and opp=="S":
    print("PLAYER WINS!!")
  elif player=="S" and opp=="P":
    print("PLAYER WINS!!")
  elif player=="R" and opp=="P":
    print("COMPUTER WINS!!")
  elif player=="P" and opp=="S":  
    print("COMPUTER WINS!!")
  elif player=="P" and opp=="R":
    print("PLAYER WINS!!")
  elif player=="S" and opp=="R":
    print("COMPUTER WINS!!")
    
