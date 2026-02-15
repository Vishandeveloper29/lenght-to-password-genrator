🔐 Python Password Generator

A simple Python program that generates a random password using lowercase letters, uppercase letters, numbers, and special characters.

📌 Features

Uses Python's built-in random module

Displays a stylized ASCII art title

Allows user to enter desired password length

Generates a secure random password

Simple and beginner-friendly project

⚙️ Requirements

Python 3.x

No external libraries required

🚀 How to Run

Clone the repository or download the project.

Open terminal or command prompt in the project folder.

Run the program:

python main.py


(Replace main.py with your actual file name if it is different.)

💻 Source Code
import random

print("""
██████╗  █████╗ ███████╗███████╗██╗    ██╗ ██████╗ ██████╗ ██████╗ 
██╔══██╗██╔══██╗██╔════╝██╔════╝██║    ██║██╔═══██╗██╔══██╗██╔══██╗
██████╔╝███████║███████╗███████╗██║ █╗ ██║██║   ██║██████╔╝██║  ██║
██╔═══╝ ██╔══██║╚════██║╚════██║██║███╗██║██║   ██║██╔══██╗██║  ██║
██║     ██║  ██║███████║███████║╚███╔███╔╝╚██████╔╝██║  ██║██████╔╝
╚═╝     ╚═╝  ╚═╝╚══════╝╚══════╝ ╚══╝╚══╝  ╚═════╝ ╚═╝  ╚═╝╚═════╝ 

                        PASSWORD
""")

chars = "abcdefghijklmnopqrstuvwxyz123456789@!#*&-_ABCDEFGHIJKLMNOPQRSTUVWXYZ"
length = int(input("Enter password length: "))
password = ""

for a in range(length):
    password += random.choice(chars)

print("Generated Password:", password)

🛠 How It Works

Imports the random module.

Defines a string containing all valid characters.

Takes user input for password length.

Uses a loop to randomly select characters.

Builds the password one character at a time.

Prints the final generated password.

🔐 Example Output
Enter password length: 10
Generated Password: aZ8@Lm2#Qp

🚀 Future Improvements

Add input validation

Use secrets module for better security

Allow user to select character types

Ensure at least one character from each category
