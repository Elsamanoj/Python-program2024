import random
def guess_the_letter():
print("welcome to the letter guessing game")
letter_to_guess
random.choice('a, z')
attempt = 0
while true:
try:
guess= input ("guess a letter between a and z:")
attempt+=1
if guess< letter_to_guess:
print("too high!try again ")
else:
print(f"congratulations!you guessed the letter correctly'{letter_to_guess}'in{attempt}attempt!")
break 
print("enter a valid letter")
