#Mini project on calculator
'''create a get method which will take and return two inputs from the user'''
def get():
    a=int(input('enter value1: '))
    b=int(input('enter value2: '))
    return a,b

#Create functions which will perform mathematical operations
def add(a,b):
    return a+b
def sub(a,b):
    return a-b
def mul(a,b):
    return a*b
def true_div(a,b):
    return a/b
def floor_div(a,b):
    return a//b
def mod(a,b):
    return a%b
def fact():
    a=int(input('enter value: '))
    fact=1
    for i in range(1,a+1):
        fact*=i
    return fact
def sqrt():
    a=int(input('enter value: '))
    return a**(1/2)
def power(a,b):
    return a**b

while True:
    print('-'*45)
    print('enter 1: addition')
    print('enter 2: subtraction')
    print('enter 3: multiplication')
    print('enter 4: true division')
    print('enter 5: floor division')
    print('enter 6: modular division')
    print('enter 7: Factorial')
    print('enter 8: Square root')
    print('enter 9: Power')
    print('enter 10: To exit the app')
    choice=int(input('enter your choice: '))
    if choice==1:
        m,n=get()
        print('The sum is: ',add(m,n))
    elif choice==2:
        m,n=get()
        print('Sub is: ',sub(m,n))
    elif choice==3:
        m,n=get()
        print('Mul is: ',mul(m,n))
    elif choice==4:
        m,n=get()
        print('True division is: ',true_div(m,n))
    elif choice==5:
        m,n=get()
        print('Floor division is: ',floor_div(m,n))
    elif choice==6:
        m,n=get()
        print('Modular division is: ',mod(m,n))
    elif choice==7:
        print('Factorial is: ',fact())
    elif choice==8:
        print('Square root is: ',sqrt())
    elif choice==9:
        m,n=get()
        print('Power is: ',power(m,n))
    elif choice==10:
        print('Thank you for using the app')
    else :
        print('Invalid choice')
