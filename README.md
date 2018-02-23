# Stone-Paper-Scissors

## The game code is written in python and it executes efficiently.

```pyhton
import random
game=["s","p","sc"]
u=""
c=""
def gaming(n):
     x=0
     y=0
     while(n>0):
          c=random.choice(game)
          print("1.Stone = s \n2.Paper = p \n3.Scissors =sc")
          u=input("Enter your choice as s,p or sc ")
          print("Computer : ",c,"\n User : ",u)
          if(c=="s"):
               if(u=="s" or u=="S"):
                    pass
               elif(u=="p" or u=="P"):
                    y=y+1
               elif(u=="sc" or u=="Sc" or u=="SC"):
                    x=x+1
               else:
                    x=x+1
          elif(c=="p"):
               if(u=="p" or u=="P"):
                    pass
               elif(u=="sc" or u=="Sc" or u=="SC"):
                    y=y+1
               elif(u=="s" or u=="S"):
                    x=x+1
               else:
                    x=x+1
          elif(c=="sc"):
               if(u=="sc" or u=="Sc" or u=="SC"):
                    pass
               elif(u=="s" or u=="S"):
                    y=y+1
               elif(u=="p" or u=="P"):
                    x=x+1
               else:
                    x=x+1
          
          n=n-1
     if(x==y):
          print("draw")
     elif(x>y):
          print("computer wins")
     else:
          print("great!! you win")
print("LET'S PLAY STONE, PAPER AND SCISSORS \n \n")
t=input("how many rounds game you want to play")
gaming(int(t))


                    
                 
