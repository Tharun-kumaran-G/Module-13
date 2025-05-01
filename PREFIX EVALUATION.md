# Exp.No:34  
## PREFIX EVALUATION

---

### AIM  
To write a Python program to evaluate a user-given Prefix expression using a stack. The expression must contain operators such as Multiplication, Addition, and Subtraction.

---

### ALGORITHM

1. **Start the program.**
2. Define a set of valid operators: `*, -, +, %, /, **`.
3. Initialize an empty stack.
4. Traverse the prefix expression from **right to left**:
   - If the character is a **digit**, convert it to an integer and push it onto the stack.
   - If the character is an **operator**, pop two elements from the stack.
     - Apply the operator on the two popped operands.
     - Push the result back onto the stack.
   - If an invalid character is encountered, raise an error.
5. After traversal, the stack should contain only **one element**.
6. Return the **single element** as the evaluation result.
7. **End the program.**

---

### PROGRAM

```
#Reg_no: 212223060288
#Name: Tharun Kumaran G

OPERATORS=set(['*','-','+','/'])

def prefix_Eval(x):
    stack=[]
    for i in x[::-1]:
        if i not in OPERATORS:
            stack.append(int(i))
        else:
            a=stack.pop()
            b=stack.pop()
            if i=='+':
                stack.append(a+b)
            elif i=='-':
                stack.append(a-b)
            elif i=='*':
                stack.append(a*b)
            elif i=='/':
                stack.append(a/b)
    return stack[0]

m=input()
print("The prefix expression is",m)
n=m.split()
print("The result is",prefix_Eval(n))

```


### OUTPUT

![image](https://github.com/user-attachments/assets/4da04974-f7d2-4b7c-92cb-ae56e705853d)

### RESULT

Thus, the python program to evaluate a user-given Prefix expression using a stack has been executed and verified successfully.
