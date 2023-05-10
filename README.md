# Memory Leak Checker

This bash script is designed to monitor and detect memory leaks in a specified process using the `leaks` command. It continuously checks the process and provides alerts if new memory leaks are detected.
Can be used with any tester

## Usage

To use this script, follow these steps:

1. Open a terminal.
2. Clone the project repository by running the following command: ```git@github.com:doffa-D/live-Memory-Leak-Detection-.git```
3. open folder by using the command: ```cd live-Memory-Leak-Detection```
4. Make the script file executable by running the command: `chmod +x leaks.sh`.
5. Run the script by executing: `./leaks.sh`.
6. When prompted, enter the PID (Process ID) of the process you want to monitor.

## Example output
```
Enter PID: 1234
[Memory Leak Detected]
    0x7f8c9b400000 (32 bytes) ROOT LEAK: <Malloc Zone> [32]
    0x7f8c9b400020 (32 bytes) ROOT LEAK: <Malloc Zone> [32]
```
## Note

Please keep in mind the following considerations:

- The script assumes that the process specified by the PID is a C program with memory leak issues. It utilizes the `leaks` command, which is specifically designed for debugging memory leaks in C programs on macOS. If you are using a different operating system or the process is not a C program, this script may not function as intended.
- Exercise caution when using this script and ensure that you have appropriate permissions to monitor the specified process.

Remember to use this script responsibly and in accordance with your system's guidelines and security practices.
