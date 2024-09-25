import random
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p',
           'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C','D', 'E', 'F',
           'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V',
           'W', 'X', 'Y', 'Z']
Symbol = ['!', '@', '#', '$', '%', '&', '^', '*', '+']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
print("Heya! Welcome to password generator")
l = int(input("How many letters you want in your password?"))#getting input from user
s = int(input("How many symbols you want in your password?"))
n = int(input("How many numbers you want in your password?"))
password = " "
for i in range(1,l+1):
    char = random.choice(letters)
    password = password+char
for i in range(1, s+1):
    password += random.choice(Symbol) #advance way
for i in range(1,n+1):
    password += random.choice(numbers)
    print(password)
