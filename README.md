# IoT-Security
Finding vulnerabilities in binary files and execute a shell

# Exercises:

Azeria Labs Stack Exercises

# Processor & OS:

- ARM-86
- Raspbian Raspberry Pi

# Notes:

# TURN OFF ASLR

-	ASLR is the mechanism that protects the memory from buffer overflows.
-	It does this by randomizing the location of the system executables are loaded into memory.
-	Command: cho 0 | sudo tee /proc/sys/kernel/randomize_va_space.


# Download GEF (GDB Enhanced Features)

-	This adds additional features to the present GDB.
-	Given more detail of while debugging the program.
-	Reference: https://blog.attify.com/demystifying-ret2zp/
-	Download From: https://github.com/hugsy/gef


