# 003 - How Does a Computer Execute a Program?

## 🎯 Goal

Understand how the CPU executes a program and how it knows which instruction to execute next.

---

## 💡 The Problem

Imagine giving someone a list of tasks:

1. Open the door.
2. Enter the office.
3. Turn on the computer.
4. Open your email.
5. Send the message.

Would they execute all tasks at once?

No.

They execute one instruction at a time.

The CPU works the same way.

---

## 🧠 Dependency

Some instructions depend on previous ones.

```dart
int a = 5;
int b = 10;
int c = a + b;

print(c);
```

`print(c)` cannot execute before `c` exists.

---

## 📍 Program Counter

The CPU contains a special register called the **Program Counter (PC)**.

Its job is to store the address of the next instruction to execute.

Example:

```text
1000 -> print("Hello");
1004 -> a = 5;
1008 -> b = 10;
1012 -> print(a + b);
```

Execution:

```
PC = 1000

↓

Execute

↓

PC = 1004

↓

Execute

↓

PC = 1008
```

---


## IF Statement

The CPU does not understand `if`.

Instead, it evaluates the condition.

If the condition is false, it skips the block and continues with the next instruction.

---

## 🧠 Engineering Insight

Understanding program execution makes debugging much easier.

Professional engineers always think about **where the execution currently is**, not just what the code looks like.

---

## 🔑 Key Concepts

- Program Counter
- Execution Flow
- Sequential Execution
- Dependency
- CPU
- Instruction

---

## 📝 Summary

The CPU executes one instruction at a time.

The Program Counter keeps track of the next instruction.

Conditional statements change the execution flow by changing where execution continues.

---

## ❓ Quiz

- What is the Program Counter?
- Why does execution happen sequentially?
- What is Dependency?
- What happens when an `if` condition is false?

---

## 🚀 Next Lesson

**004 - How Does IF Actually Work?**