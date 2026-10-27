history = []
memory = 0
last_result = 0

while True:
    command = input("type command:")

    if command =="h":

        for item in history:
            print(item)

    elif command =="b":
        print("Binary:", bin(int(last_result))) 

    elif command =="o":
        print("Octal:", oct(int(last_result)))  

    elif command =="x":
        print("hexadecimal:", hex(int(last_result))) 

    elif command =="m+":
        memory = memory + last_result
        print("Memory:", memory)

    elif command =="m-":
        memory = memory - last_result
        print("Memory:", memory)

    elif command =="m":
        print("Memory:", memory)

    elif command =="q":
        break

    else:
        num1 = float(command)
        op = input("Operator:")
        num2 = float(input("type num2:"))

        if op == "+":
            last_result = num1 + num2
        elif op == "-": 
            last_result = num1 - num2
        elif op == "*":
            last_result = num1 * num2
        elif op == "/":
            if num2 == 0:
                print("error num2==0!")
                #print(" تقسیم بر صفر امکان پذیر نیست")
                continue
            last_result = num1 / num2
        elif op == "**":
            last_result = num1 ** num2
        else:
            print("error Operator!")
            #print("عملگرد نامعتبر است!")
            continue
        print("Result:", last_result)

        history.append(
            str(num1) + " " + op + " " +
            str(num2) + " = " + str(last_result)
         )