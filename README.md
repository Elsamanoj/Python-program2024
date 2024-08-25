import random
def guess_the_letter():
    print("Welcome to the letter guessing game!")
    letter_to_guess = random.choice('abcdefghijklmnopqrstuvwxyz')
    
    attempt = 0
    
    while True:
        try:
            guess = input("Guess a letter between 'a' and 'z': ").lower()
            attempt += 1
            
            if not guess.isalpha() or len(guess) != 1:
                print("Enter a valid single letter.")
                continue
            
            if guess < letter_to_guess:
                print("Too low! Try again.")
            elif guess > letter_to_guess:
                print("Too high! Try again.")
            else:
                print(f"Congratulations! You guessed the letter correctly: '{letter_to_guess}' in {attempt} attempt(s)!")
                break
        
        except Exception as e:
            print("An error occurred:", e)

guess_the_letter()
