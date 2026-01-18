# Introduction to C Programming

**Difficulty:** Beginner  
**Estimated Time:** 30 minutes  
**Prerequisites:** None - this is your first lesson!

## 🎯 What You'll Learn
- What is C and why it's important
- Your first C program
- How to compile and run C code
- Basic program structure

## 📖 Introduction

C is one of the most important programming languages ever created. It was developed in the 1970s and is still widely used today for:

- **Operating Systems** (Linux, Windows)
- **Embedded Systems** (phones, cars, appliances)
- **Game Engines**
- **High-performance applications**

Learning C gives you a deep understanding of how computers actually work!

## 🔧 Why Learn C?

- ✅ Understand memory and hardware
- ✅ Foundation for C++, C#, Java
- ✅ Fast and efficient
- ✅ Works on minimal hardware
- ✅ Used everywhere in the world

## 💻 Your First C Program

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

### Let's Break It Down:

1. **#include <stdio.h>**
   - Includes standard input/output library
   - Gives us printf() function

2. **int main()**
   - Every C program starts here
   - "int" means it returns a number

3. **printf("Hello, World!\n")**
   - Prints text to screen
   - \n means "new line"

4. **return 0**
   - Tells computer: program finished successfully
   - 0 = success

## 📱 Running on Mobile

### Using C4droid (Android):
1. Open C4droid app
2. Copy the code above
3. Tap "Compile & Run"
4. See "Hello, World!" appear!

### Using Pydroid 3 with C:
1. Install C compiler in app
2. Create new .c file
3. Paste code
4. Run!

## ✅ Practice Exercises

### Exercise 1: Change the Message
Modify the program to print your name:
```c
printf("Hello, my name is [YOUR NAME]!\n");
```

### Exercise 2: Multiple Lines
Print three lines of text:
```c
printf("Line 1\n");
printf("Line 2\n");
printf("Line 3\n");
```

### Exercise 3: Add More
Can you print your name, age, and where you're from?

## 🎯 Mini Project

Create a program that introduces yourself:
- Your name
- Your age
- Where you live
- What you want to learn

Example output:
```
Hello! I'm Amara
I am 16 years old
I live in Lagos
I want to learn programming!
```

## 📚 Next Steps

- [Lesson 02: Variables and Data Types](02-variables.md)
- [Practice: More printf exercises](../projects/beginner/hello-variations.md)

## ❓ Common Questions

**Q: Do I need a computer to learn C?**  
A: No! You can use mobile apps like C4droid or online compilers.

**Q: Is C hard to learn?**  
A: C is powerful but straightforward. Take it step by step!

**Q: Why does my program need return 0?**  
A: It tells the operating system the program finished correctly.

**Q: What does #include mean?**  
A: It includes code libraries that add more functions to your program.

---

**Made with 💙 by the Afrowave Community**

[← Back to C Programming](README.md) | [Next Lesson →](02-variables.md)