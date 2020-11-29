### Hi there 👋
My name is Chloe and I am currently working as an IT Technician in the U.K.

![](https://media1.tenor.com/images/ef6dc1481b862291961bc37b6d7ff064/tenor.gif)

- 💻 Coding
- 🎧 Music 
- ☕ Coffee
- ⚔️ Games
- 🍕 Pizza

My latest code for a Password Generator written in Python 🐍

```py
import random
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the Password Generator!")
nr_letters= int(input("How many letters would you like in your password?\n")) 
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))

lst = []

for i in range(1, nr_letters + 1):
    lst.append(random.choice(letters))
for i in range(1, nr_symbols + 1):
    lst.append(random.choice(symbols))
for i in range(1, nr_numbers + 1):
    lst.append(random.choice(numbers))
random.shuffle(lst)

for l in lst:
    password = "".join(lst)
print(password)
```
