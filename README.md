import random
uppercase = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
lowercase = "abcdefghijklmnopqrstuvwxyz"
number = "0123456789"
special = "!@#$%^&*()[]|:'<>,?"

all_characters = uppercase + lowercase + number + special

length = int(input("Enter Password Length: "))
password = ""
for i in range(length):
    password += random.choice(all_characters)

print("\nGenerated Password: ", password)
