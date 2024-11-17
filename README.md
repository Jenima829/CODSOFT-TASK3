NAME: JENIFER Y
DOMAIN : PYTHON PROGRAMMING
TASK 3: PASSWORD GENERATOR

Here is the explanation of my project,
Introduction:
This Python script is a personalized tool designed to create random, secure passwords based on user preferences. The code allows the user to customize the password's length and its inclusion of digits and special characters.
Code Breakdown:
Importing Required Modules:

python
Copy code
import random
import string
random is used for generating random characters.
string provides predefined sets of characters like letters, digits, and punctuation.

Defining the Password Generation Function:
def generate_password(length, use_digits, use_special):
    characters = string.ascii_letters
    if use_digits:
        characters += string.digits
    if use_special:
        characters += string.punctuation
    return ''.join(random.choice(characters) for _ in range(length))
length: The desired length of the password.
use_digits: Whether to include digits (True or False).
use_special: Whether to include special characters (True or False).
characters: Initializes with alphabet letters and dynamically adds digits and special characters based on user input.
The function uses a list comprehension to pick random characters from the characters string for the specified length.

User Input and Validation:
python
Copy code
length = int(input("Enter the desired length of the password: "))
use_digits = input("Include digits? (yes/no): ").strip().lower() == 'yes'
use_special = input("Include special characters? (yes/no): ").strip().lower() == 'yes'
Prompts the user for password length.
Converts user inputs about including digits and special characters into boolean values by comparing the input to 'yes'.

Generating and Displaying the Password:
password = generate_password(length, use_digits, use_special)
print("Generated Password:", password)
Calls the generate_password function with user inputs.
Prints the randomly generated password.

Conclusion
This script, which I developed, is an efficient and flexible way to generate passwords tailored to user needs. By leveraging Python's random and string modules, it ensures strong, randomized passwords that meet desired criteria for security.

OUTPUT:


<img width="298" alt="password" src="https://github.com/user-attachments/assets/c34b8485-1cae-4f25-9e36-cc6aef519fde">












