Command Line Arguments:
"sys" is the module used to read the command line arguments
sys will install by default in the pyhton installations, you need to install it using the pip command
example:
import sys 
def add(num1,num2):
    a = num1 + num2
    return a 
def sub(num1,num2):
    s = num1 - num2
    return s
def mul(num1,num2):
    m = num1 * num2
    return m
def div(num1,  num2):
    d = num1 // num2
    return d

num1 = float(sys.argv[1])
operation = sys.argv[2]
num2 = float(sys.argv[3])

if operation == "add":
    output = add(num1,num2)
    print(output)

if operation == "sub":
    output = sub(num1,num2)
    print(output)
if operation == "mul":
    output = mul(num1,num2)
    print(output)
if operation == "div":
    output = div(num1,num2)
    print(output)
In command line enter python filename arguments like python func.py 2 add 3, you can see the output as 5

Environment Variables:
When you are having the sensitive information that need to be used in the code you can go with the environment variables.
env: command is used to diaplay the env varibles 
export password="venkat" : to create/store a environment variable
import os #os module is used to get the environment variables
print(os.getenv("password")) 

after the code execute as python filename.py you will get the stored password this can be used for tokens also.
This can be used any time if you need to stotre the sensitive info and to be passed them in the code with privacy.


 
