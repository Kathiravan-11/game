import random
print("welcome to rock,paper, scissors game")
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''
paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
game_image=[rock,paper,scissors]
user=int(input("choose 0 for rock,1 for paper and 2 for scissors"))
if user>=3:
    print("you have typed invalid number you lose")
else:
  print("user chose")
  print(game_image[user])

  computer_choice=random.randint(0,2)
  print("computer chose")
  print(game_image[computer_choice])
  if user==0 and computer_choice== 2:
    print("you win")
  elif user==2 and computer_choice==0:
    print("you lose")
  elif user==3 and computer_choice==1:
    print("you win")
  elif user==computer_choice:
    print("its draw")
  elif user>computer_choice:
    print("you win")
  elif user<computer_choice:
    print("you lose")

