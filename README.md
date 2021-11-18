- # EXERCISE 1 – Simple counting loops
2	- # Can you create a for loop that prints 2, 5, 8, 11, 14? 
3	- for i in range(2,15,3): 
4	-   print(i) 
5	-
6	- # Can you create a while loop that does the same thing? 
7	- i = 2
8	- while i <= 14:
9	-   print(i)
10	-   i = i + 3
11	-
12	- # EXERCISE 2 – Loop that prints the SUM of numbers from 1 to inputted value
13	-
14	- sum = 0
15	- value = int(input("Enter number up to 100: "))
16	- for i in value:
17	-   if value > 100:
18	-     print("No.") 
19	-
20	- # EXERCISE 3 – In class we created code to sum the three-game total for bowling 
21	- highest_score = 0
22  - total_score = 0
23  - for i in range(3):
24  -  my_score = int(input("Enter a number: "))
25  -  if my_score < 0 or my_score > 300:
26  -    print("Invalid input, you get a 0!")
27  -    my_score = 0
28  -  if my_score > highest_score:
29  -    highest_score = my_score
30  -  total_score += my_score
31  -  print("The 3 game total is:", total_score)
32  -  print("your high game is:", highest_score)
26	-
271	  # EXERCISE 4 – Create a loop that does the following 
import random
hp = 100
damage = 0

complete = False
while not complete:
  cont = input("Do you want to continue? (y/n): ")
  if cont == "y" or "yes":
    damage = random.randint(0,100)
    hp -= damage
  if hp <= 0:
    print("Game Over, start trying")
    complete = True
  else:
    print("You were damaged by", damage, "and your HP is now", hp)
  if cont == "n" or "no":
    complete = True
  else:
    print("Invalid input stoopid.")
29	- # EXCERCISE 5 - Using nested for loops, create code that outputs the following:
30	- homework = "No homework tonight, please"
31	- for i in range(5):
32	-   print(homework)
33	-   homework = homework + " please,"
34	-
35	- # EXERCISE 6 – Use a while loop to write a program that repeatedly simulates a coin flip and asks the user to guess heads or tails. Once the user guesses incorrectly, the program prints the number of correct guesses and terminates.
362	  import random 
3	+ damage = 0 
374	 
38	- correct = True 
39	- while correct: 
40	-   flip = random.randint(0,1) 
41	-   guess = int(input("Heads/Tails?(h=1/t=0) ")) 
5	+ hitpoints = 100
6	+ another = int(input("Another round? (y/n): "))
7	+ if another == y:
8	+   print(random.hitpoints)
42	-   if flip != guess: 
43	-     print("WRONG") 
44	-     correct = False 
