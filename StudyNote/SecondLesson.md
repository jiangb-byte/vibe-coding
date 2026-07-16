# Lessson 2 GCC Practice
```
1. Install gcc on any Linux environment (Ubuntu/Rocky Lab or Windows WSL).
2. Write a basic C program using vi, and ensure you fully understand every line of code. 
3. Compile it with gcc and observe the 4 distinct stages: preprocessing, compilation, assembly, and linking.
4. Run the program and monitor it via the top command.
5. Grasp the fundamental differences between a program and a process.
6. Summarize your learnings into technical notes and push the notes and source code to GitHub.

```

### Install GCC on WSL2

1. In WSL, run 
   1. sudo apt update && sudo apt upgrade -y
2. Install GCC and Development Tools
   1. sudo apt install build-essential gdb -y  *(This command installs gcc (C compiler), g++ (C++ compiler), make, and gdb (debugger))*

```c
#include <stdio.h>
int main()
      {
      printf ("GCC is working on WSL!\n");
      return 0;
      }
```
 
### Program vs Process
|Feature|Program|Process|
| ---  | --- | --- |
|State |Passive (resides quietly on your storage disk)|Active (loaded into RAM and executing)|
| Lifespan  | Persistent (exists until you manually delete the file) | Temporary (exists only from execution to termination) |
| Resources  | Consists only of physical disk space | Consists of CPU time, RAM, file descriptors, and I/O devices |
| Representation  | An executable file (e.g., in ELF format in Linux) or a script | Represented by a unique PID (Process ID) and a PCB (Process Control Block) in the kernel |
| Relationship  | 1-to-Many: One program can be used to spawn many processes | An active, isolated instance of that program
 |

