- Summary of each chapter is great. it's really __summary__
- the page of Chapter 7 is wrong. use content table to jump
- 
# Part I Virtualization
## The Abstraction: The Process

### Processes

#### what parts of the machine are important to the execution of this program

- memory
- register
  - program counter (PC)
  - stack pointer
  - frame pointer
- IO

#### Process Creation

- the code and static data are loaded into memory

- initial stack

- initial heap

- others

  - IO

- jump to entry point, main()

### CPU Virtualization

- Basic idea: time sharing

  - challenges

    - performance
    - control

#### Basic Technique: Limited Direct Execution
- Without Limits--the os just like library
- 
#### Problem #1: Restricted Operations

- user mode
- kernel mode
- traps and trap table
#### Problem #2: Switching Between Processes
- THE CRUX: HOW TO REGAIN CONTROL OF THE CPU

- A Cooperative Approach: Wait For System Calls

- A Non-Cooperative Approach: The OS Takes Control

- Saving and Restoring Context

  ![context_swtich](/image/Three.Easy.Pieces/context_switch.png)
#### Concurrency problem
- disable interrupts
- locking
- 
- mechanisms
  -  low-level machinery
  - context switch
- policies
  - scheduling policy 


###  Memory Virtualization

### Scheduling: Proportional Share
#### lottery scheduling
#### stride scheduling
#### CFS
- a bit like weighted round-robin with dynamic time slices
- [Linux CFS调度器](https://zhuanlan.zhihu.com/p/56430999)

# Part II Concurrency
# Part III Persistence


# Part 5 security
## 54 Authentication
- Authentication by What You Know
- Authentication by What You Have
- Authentication by What You Are
## 55 Access Control
- access control list system - ACL
  - linux, user/group/other, rwx
- capability-based system
  - key or ticket



