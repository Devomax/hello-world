# hello-world

number = random.randint(1, 10)
tries = 1

uname = input("Hello, what's your name?")
print("hello", uname + ".")

question = input("Would you like to play a game? [Y/N] ")
if question == "n":
	print("oh..Ok")

if question == "y":
	print("I'm thinking of a number berween 1 & 10")
	guess = int(input("Have a guess"))
	if guess > number:
		print("Guess lower")
if guess < number:
		print("Guess higher")
while guess != number:
	tries += 1
	guess = int(input("Try agin:"))
	if guess < number:
		print("Guess higher")
if guess == number:
	print("you're right! you win! The number was", number, \
		  "and it only", tries, "isku day!")
	
