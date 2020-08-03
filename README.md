# OTP-Generator
#1

#first-creating the four digit OTP using function
#it is important to import the random library to generate random 4 digit OTP numbers

import math, random
def OTPgen(n):
		digits = "0123456789"
		OTP = ""
    for i in range(n):
				OTP += digits[math.floor(random.random()*10)]
		return OTP
#main function
print("The 4 digit OTP is: ",OTPgen(4))

#In the above example i have put the range for the 4 digit OTP, similarly we can change the range as 5 or 3 and so on.

#2

#Lets write a code without using function
#Here lets import both random and randint
#Randint gives the random integers described within a range

import random
from random import randint
OTP=random.randint(1000,9999)
print("The four digit OTP is: ",OTP)

#Similarly we can modify the range for 3 digit, 5 digit otp and so on.
