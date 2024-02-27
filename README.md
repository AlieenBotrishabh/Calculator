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
