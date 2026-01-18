# Introduction to Assembly Language

**Difficulty:** Beginner  
**Estimated Time:** 45 minutes  
**Prerequisites:** Basic understanding of binary and hexadecimal numbers

## 🎯 What You'll Learn
- What assembly language is and why it matters
- How assembly relates to machine code
- Basic concepts: registers, instructions, memory
- Your first assembly program

## 📖 Introduction

Assembly language is the lowest-level programming language humans can reasonably read. It's one step above raw binary machine code.

**Why learn Assembly?**
- 🧠 Understand how computers really work
- ⚡ Write extremely fast code
- 🔧 Debug low-level problems
- 💪 Become a better programmer in ANY language

**Real-world uses:**
- Operating system kernels
- Device drivers
- Embedded systems (phones, cars, IoT)
- Game console programming
- Performance-critical code

## 🏗️ How Computers Execute Code

### The Journey from Code to Execution

```
High-Level Code (C, JavaScript)
        ↓
    Compiler
        ↓
Assembly Language ← We are here!
        ↓
   Assembler
        ↓
Machine Code (Binary)
        ↓
    CPU Executes
```

## 🧠 Basic Concepts

### 1. Registers
Think of registers as the CPU's **super-fast temporary storage**.

Common x86-64 registers:
- `rax` - Accumulator (math operations)
- `rbx` - Base register
- `rcx` - Counter (loops)
- `rdx` - Data register
- `rsi` - Source index
- `rdi` - Destination index
- `rsp` - Stack pointer
- `rbp` - Base pointer

**Analogy:** If RAM is a warehouse, registers are your hands - tiny storage but instantly accessible.

### 2. Instructions
Assembly uses simple commands:
- `mov` - Move data
- `add` - Addition
- `sub` - Subtraction
- `jmp` - Jump to another location
- `cmp` - Compare values

### 3. Memory
Data is stored in memory addresses:
```
Address    Value
0x1000  →  42
0x1004  →  100
0x1008  →  255
```

## 💻 Your First Assembly Program

### Hello World (x86-64 Linux)

```asm
section .data
    msg db 'Hello, Afrowave!', 0xA
    len equ $ - msg

section .text
    global _start

_start:
    ; Write message to stdout
    mov rax, 1      ; syscall: write
    mov rdi, 1      ; file descriptor: stdout
    mov rsi, msg    ; message address
    mov rdx, len    ; message length
    syscall         ; call kernel

    ; Exit program
    mov rax, 60     ; syscall: exit
    mov rdi, 0      ; exit code 0
    syscall
```

### Understanding Each Line

```asm
section .data
```
- Defines the data section (constants)

```asm
msg db 'Hello, Afrowave!', 0xA
```
- `msg` = label (name for this data)
- `db` = "define bytes"
- `0xA` = newline character (hex 10)

```asm
len equ $ - msg
```
- Calculate message length
- `$` = current position
- `$ - msg` = length

```asm
mov rax, 1
```
- Move value 1 into register `rax`
- This selects the "write" system call

```asm
syscall
```
- Ask the operating system to do something
- What it does depends on `rax` value

## 🔢 Working with Numbers

### Simple Addition

```asm
section .text
    global _start

_start:
    mov rax, 5      ; rax = 5
    mov rbx, 3      ; rbx = 3
    add rax, rbx    ; rax = rax + rbx = 8
    
    ; rax now contains 8
```

### Subtraction

```asm
mov rax, 10     ; rax = 10
sub rax, 4      ; rax = rax - 4 = 6
```

### Multiplication

```asm
mov rax, 6      ; rax = 6
mov rbx, 7      ; rbx = 7
imul rax, rbx   ; rax = rax * rbx = 42
```

## 📱 Mobile-Friendly Learning

**Can I run Assembly on my phone?**

Not easily for x86, but you can:
- ✅ Learn ARM assembly (phones use ARM)
- ✅ Use online emulators
- ✅ Study the concepts
- ✅ Use tools like Termux (Android)

**Recommended mobile tools:**
- **Online:** godbolt.org (Compiler Explorer)
- **Android:** Termux + GCC
- **iOS:** Read and study (iOS restricts execution)

## ✅ Practice Exercises

### Exercise 1: Modify Hello World
Change the message to print your name.

### Exercise 2: Calculate
Write code that:
1. Sets `rax` to 15
2. Sets `rbx` to 3
3. Subtracts `rbx` from `rax`
4. Stores result in `rcx`

**Hint:**
```asm
mov rax, 15
mov rbx, 3
sub rax, rbx
mov rcx, rax
```

### Exercise 3: Understanding
What does this code do?
```asm
mov rax, 10
mov rbx, 20
add rax, rbx
add rax, rbx
```

**Answer:** rax = 10 + 20 + 20 = 50

## 🎯 Mini Project: Number Doubler

Write a program that:
1. Stores number 7 in `rax`
2. Doubles it (adds it to itself)
3. Result should be 14 in `rax`

**Solution:**
```asm
section .text
    global _start

_start:
    mov rax, 7      ; Start with 7
    add rax, rax    ; Double it: 7 + 7 = 14
    
    ; Exit
    mov rax, 60
    mov rdi, 0
    syscall
```

## 🧩 Key Differences: AT&T vs Intel Syntax

There are two ways to write assembly:

**Intel Syntax (easier to read):**
```asm
mov rax, 5      ; destination, source
```

**AT&T Syntax (Linux default):**
```asm
movq $5, %rax   ; source, destination
```

This course uses **Intel syntax** (clearer for beginners).

## 📚 Next Steps

**After this lesson:**
1. ➡️ [Working with Registers](./02-registers-deep-dive.md)
2. ➡️ [Memory Addressing](./03-memory-addressing.md)
3. ➡️ [Control Flow (Jumps and Loops)](./04-control-flow.md)

**Additional resources:**
- [Binary and Hexadecimal](../theory/binary-hexadecimal/01-number-systems.md)
- [Computer Architecture](../theory/computer-architecture/01-cpu-basics.md)

## ❓ Common Questions

**Q: Is Assembly hard?**  
A: It's different, not harder. You're closer to the hardware, so things are more explicit.

**Q: Which Assembly should I learn?**  
A: Start with x86-64 (most common) or ARM (for mobile/embedded).

**Q: Do I need Assembly for web development?**  
A: No, but understanding it makes you a better programmer.

**Q: Can I use Assembly on my phone?**  
A: You can learn and study it. Practical execution requires specific tools.

## 🏆 What You've Learned

✅ What assembly language is  
✅ Registers, instructions, and memory  
✅ Your first assembly program  
✅ Basic arithmetic operations  
✅ How code becomes machine instructions

---

**Continue learning:** [02-registers-deep-dive.md](./02-registers-deep-dive.md)

**Made with 💙 by the Afrowave Community