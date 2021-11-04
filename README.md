# AHC-application-process
# Riley Skertich
# This program is to help my family business
# My parents own a physician recruitment company
# a big part of their job is to take applications on doctors
# Creating them a system that allows them to enter the information easily
# Title of project/ application
print("Candidate Application form")
# For position, I am looking for the hospital name
position = input("AHC Position Applied for ")
# The source should be one of the many websites we work with (DocCafe, Indeed)
source = input("Source ")
name = input("Doctors first and last name ")
speciality = input("Speciality you are looking for ")
email = input("Doctors email address ")
citizenship = input("Current Citizenship status ")
status = input("MD or DO ")
pronouns = input("Preferred pronouns ")
# Usually when taking an interview, the above is bunched together as a heading
# I will "print" out each section of the interview out in different sections
# I will add end = '' to each print statement so it prints out as a paragraph
# I add a space after the comma so it separates each sentence
print(name + "(" + status + ")" + " is looking for a " + speciality +
      " position" + ". ", end='')
print(pronouns + " email address is " + email + ". ", end='')
print(pronouns + " applied for " + position + " through " + source + ". ",
      end='')
print(pronouns + " is a " + citizenship + " citizen" + ". ")

date = input("Date interviewed: ")
availability = input("Date available: ")
graduation = int(input("Graduation year: "))
licenses = input("What states are you licensed in? ")
languages = input("Languages Spoken: ")
print(pronouns + " speaks " + languages + ".")
print(pronouns + " is licensed in " + licenses + ".")
print(name + " was interviewed on " + date + ". " + pronouns +
      " is available to start on " + availability + ".")
# defining debt
debt = float(input("How much medical debt are you in? "))
# if statement will run if user is in 0 debt
# == is used to check whether two expressions give same value
# if debt is equal to zero or they are in negative debt, the if statement runs
if debt == 0 or debt < 0:
    print("Congrats, you are in no medical debt!")
# if debt is greater then 0 and less than 100000, the elif statement will run
elif not debt > 100000:
    print("It will be easy to find you a position to take care of your debt")
# if debt is greater then or equal to 100000 and not equal to zero,
# then elif statement will run
# != means does not equal
elif debt <= 200000 and debt != 0:
    print("We will search for positions that take care of debt")
else:
    print("Too much debt.")


# We now want to learn more about the physicians desired practice
# For setting, we are looking for an answer like clinic, private practice, etc.
# Created a menu
# def defines a menu
def menu():
    incorrectInput = True

# While true will run the loop until it "breaks"
    while incorrectInput:
        print("What is your preferred practice setting? ")
        print("Hospital employment")
        print("Group practice")
        print("Solo")
        print("Academic")
        print("Open")
        setting = input()
# if statement will run if user types "Hospital employment"
# The loop will stop running if the user types any of the menu options
        if setting == "Hospital employment":
            print("Your preferred practice setting is hospital employment")
            incorrectInput = False
# elif statement is saying if previous are not true try this statement
# used w3schools for definitions about elif and else
        elif setting == "Group practice":
            print("Your preferred practice setting is group practice")
            incorrectInput = False
        elif setting == "Solo":
            print("Your preferred practice setting is solo")
            incorrectInput = False
        elif setting == "Academic":
            print("Your preferred practice setting is academic")
            incorrectInput = False
        elif setting == "Open":
            print("Your preferred practice setting is open")
            incorrectInput = False
# else statement runs if anything but the if or elif statements is entered
        else:
            print("Invalid selection. Try again.")


menu()
# in or outpatient (chose one)
in_outpatient = input("What is your in and outpatient preference? ")
# For call preference we are looking for a ratio (1:5)
call = input("What is your call preference? ")
# by setup I mean days on and days of (eg. 5 days on 5 days off)
setup = input("What is your ideal setup? ")
# looking for an approximate number of people the doctor wants to see per day
patients = input("What is your desired number of daily patients visits? ")
# technology you prefers to have or need
technology = input("What is your preferred technology? ")
# skills should include what procedures you typically do
print(pronouns + " prefers " + in_outpatient + " preference.", sep='')
print(pronouns + " has a call preference of " + call + ".")
print(pronouns + " ideal setup is " + setup)
print(pronouns + " wants to see " + patients + " a day.")
print(pronouns + " preferred technology is " + technology + ".")
# x in range will print the code the amount of times in the range function
# I want to find users top three procedures so I repeat the prompt three times
print("What are your top three procedures?")
top_procedures = ""
for x in range(3):
    top_procedures += input(" Procedure: ")
print(top_procedures)

print("Thank you for taking the time to fill out this application.")
print("We will be in contact with you shortly")
# I can copy and paste this information into our other system
# This program helps manages our time better
# I now am going to give the user some information about me
# Each number is going to be one number part of my phone number
# ** is squaring the number
num1 = 2 ** 3
# * is multiplying
num2 = 2 * 2
# / is dividing
# The int() is printing the number without a decimal
num3 = int(49 / 7)
# + is adding the numbers
num4 = 5 + 3
# - is subtracting the numbers
num5 = 8 - 3
# % is modulus, returns the remainder
num6 = 4 % 4
# // is floor division, it divides two numbers and rounds down to an integer
num7 = 82 // 9
num8 = 6
num9 = 3
phoneNumber = num1, num2, num3, num4, num5, num6, num7, num8, num9, num5
print("I can be reached at: #", num1, num2, num3, num4, num5, num6, num7,
      num8, num9, num5, sep='')
# I give them my number to contact me
print("Bye " * 2)
