# Exp.No:31  
## IMPLEMENTATION OF STACK

---

### AIM  
To write a Python program to implement a stack using a list and its built-in methods (`append()`, `pop()`).

---

### ALGORITHM

1. **Start the program.**
2. **Define a class `st`** with the following methods:
   - `push(self, num)`: Adds the number `num` to the stack.
   - `pop(self)`: Removes and returns the top element from the stack.
3. **Create a stack object `s`** using the class `st`.
4. **Input the stack size**: Take an integer input `size` to define the size of the stack.
5. **Loop through numbers from 1 to size**: Add only the odd numbers to the stack using the `push()` method.
6. **Display the elements** in the stack after the loop completes.
7. **Call `pop()`** to remove the top element from the stack and display the popped element.
8. **Display the stack again** to show the remaining elements.
9. **End the program.**

---

### PROGRAM

```
#Reg_no: 212223060288
#Name: Tharun Kumaran G

stack = []
class st:
    def push(self,S):
        for i in S:
            stack.append(i)
        return
        
    def pop(self):
        if stack:
            print("Element popped : ",stack.pop())
        else:
            print("The stack is empty")
        return
    
    def peek(self):
        print("Elements in the stack\n",stack)
        return
        
s=st()
size=int(input())
l=[i for i in range(1,size) if i%2!=0]
s.push(l)
s.peek()
s.pop()
s.peek()
```

### OUTPUT

![image](https://github.com/user-attachments/assets/23794658-ca22-4490-9991-e9282132d5db)

### RESULT

Thus, the python program to implement a stack using a list and its built-in methods (`append()`, `pop()`) has been executed and verified successfully.
