# Rock-Paper-and-Scissor-Game
Python Program Project

import random
print('__________________ \n')
print('**//** Games rule of Rocks,Paper,Scissor:- **//**\n')
print('__________________ \n')
print('Rocks Vs Paper = Paper wins \n')
print('Rocks Vs Scissor = Rock wins \n')
print('Scissor Vs Paper = Scissor wins \n')
print('If both player getting same then game will Die \n ')
while True:
print('__________________ \n')
print('### Enter your choice ##### \n 1. Rock \n 2. Paper \n 3. Scissor\n')
print('__________________ \n')
choice = int(input('Your turn: '))
while choice >3 or choice <1 :
choice = int(input('enter input'))
if choice == 1:
choice_name = 'Rock'
elif choice == 2:
choice_name = 'Paper'
elif choice == 3:
choice_name = 'Scissor'
else:
print('please enter valid input')
print('your choice is: ',choice_name)
print('Now its computer turn')
comp_choice = random.randint(1,3)
while comp_choice == choice:
comp_choice = random.randint(1,3)
if comp_choice == 1:
comp_choice_name = 'Rock'
elif comp_choice == 2:
comp_choice_name = 'Paper'
elif comp_choice == 3:
comp_choice_name = 'Scissor'
else:
print('please give valid input')
print('computer choice is', comp_choice_name)
print(choice_name, 'Vs', comp_choice_name)
if((choice == 1 and comp_choice == 3) or (choice == 3 and comp_choice == 1)):
print('<= Rocks wins =>\n',end = ' ')
result = 'Rocks'
elif((choice == 1 and comp_choice == 2) or (choice == 2 and comp_choice == 1)):
print('<= Paper wins =>\n',end = ' ')
result = 'Paper'
elif((choice == 2 and comp_choice == 3) or (choice == 3 and comp_choice == 2)):
print('<= Scissor wins =>\n',end=' ')
result = 'Scissor'
else:
print()
if result == choice_name:
print('______****_______ \n')
print(' |||| YOU WINS |||| \n')
print('______****_______ \n')
else:
print('<==Computer Wins, Better luck next time ==>')
print('Do you want to play again ? (y/n)')
ans = input()
if ans == 'n' or ans == 'N':
break
print('\n #### Thanks for playing ####')
