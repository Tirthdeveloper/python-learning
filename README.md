# python-learning

print("WELCOME TO THE PATTERN GENERATOR AND NUMBER ANALYZER")
print("")
print("")
print("select an option:")
print("1.generate a pattern")
print("2.analyze a numbers")
print("3.exit")
option=int(input("Enter Your Option: "))
if option==1:
    n=int(input("Enter number of rows for the pattern: "))
    for x in range(1,11):
        for y in range(1,x+1):
            print("*",end=" ")
        print("")
elif option==2:
    a = int(input("Enter the start number: "))
    b = int(input("Enter the end number: "))
    sum = 0
    for i in range(a, b+1, 1):
        if i % 2 == 0:
            print(f"Number {i} is even")
            sum=sum+i
        else:
            print(f"Number {i} is odd")
            sum = sum + i 

        print(f"Sum of all numbers from {a} to {b} is: {sum}")
        
elif option==3:
        print("exiting the program.   GOODBYE!")
else:
    print("invalid option. please try again.")
