
if-else statement:

python
Copy code
if choice == '+':
    print(a)
This if statement checks if the value of the variable choice is equal to '+'.
If the condition is true, it executes the code block inside the if statement.
In this case, it prints the value of variable a, which corresponds to the result of addition (c1) from the cal function.
Multiple Return Statements:

python
Copy code
return c1, d1, e1, f, g
The cal function has a single return statement, but it returns multiple values separated by commas.
This is possible in Python because the return statement can return a tuple (or any other sequence) of values.
In this case, the function returns a tuple containing the results of five mathematical operations: c1 (addition), d1 (subtraction), e1 (multiplication), f (division), and g (exponentiation).
When you call the cal function and assign its return value to multiple variables (a, b, c, d, e), Python unpacks the returned tuple and assigns each element to its corresponding variable.
So, in summary, the if-else statement in the code checks the user's choice of operation, and based on that choice, it prints the corresponding result of the mathematical operation performed by the cal function. The cal function utilizes multiple return statements to return the results of multiple operations simultaneously.


def cal(x, y):
    c1 = x + y
    d1 = x - y
    e1 = x * y
    f = x / y
    g = x ** y
    return c1, d1, e1, f, g


if __name__ == "__main__":
    choice = str(input("Enter your choice"))
    a1 = int(input("Enter the value"))
    b1 = int(input("Enter the value"))
    a, b, c, d, e = cal(a1, b1)
    if choice == '+':
        print(a)

    elif choice == '-':
        print(b)

    elif choice == '*':
        print(c)

    elif choice == '/':
        print(d)

    elif choice == '**':
        print(e)

    else:
        print("Wrong choice")
