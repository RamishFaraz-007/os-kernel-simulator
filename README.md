# 🧠 Operating System Kernel Simulator

This is a **modular Operating System Kernel Simulator** developed in **C on Ubuntu Linux**.  
The project simulates core kernel functionalities such as **process management, CPU scheduling, and memory allocation**.

This project was developed as part of the **Operating Systems Lab (CE332L)** at Air University.

---

## 🎯 Objective
To simulate the internal working of an operating system kernel and demonstrate how processes compete for CPU time and memory resources.

---

## ⚙️ Features

### Process Management
- Process Control Block (PCB)
- Process states:
  NEW → READY → RUNNING → TERMINATED
- Supports up to 10 processes

### CPU Scheduling Algorithms
- First Come First Served (FCFS)
- Shortest Job First (SJF)
- Priority Scheduling
- Round Robin (Time Quantum based)

Automatically calculates:
- Waiting Time
- Turnaround Time
- CPU Utilization
- Throughput

### Memory Management
- Simulated RAM (up to 256 units)
- Allocation strategies:
  - First Fit
  - Best Fit
  - Worst Fit

### Terminal Interface
- Color-coded process states using ANSI escape codes
- Gantt Chart visualization
- Menu-driven interaction

---

## 🏗 File Structure

main.c → Main controller  
process_mgr.c → Process management  
scheduler.c → Scheduling algorithms  
memory_mgr.c → Memory allocation  
shared.h → Global definitions  
Makefile → Build automation  

---

## 🛠 Technologies Used
- Language: C (C11)
- OS: Ubuntu Linux
- Compiler: GCC
- Build Tool: Make
- Virtual Machine: VirtualBox
- Environment: Vagrant

---

## ▶️ How to Run
```bash
make
./simulator
