# Strict two-phase locking (S2PL) protocol
This project implement the strict two-phase locking (S2PL) protocol with shared 
locks for read and exclusive locks for write in the transaction manager.

# How to run this project:

This project make use of makefile and tmtest file to compile and run the code.

## Running project on Linux

1. Download make command:
```
sudo apt update
sudo apt install make
```

2. Get inside the src folder, run the following command to clear the compiled classes:
```
make clean
```
This command will compile the code in src folder

3. Run this command to make the executable:
```
make zgt_test
```
4. Run this command to run the program n times(since there will be race conditions(obvious because of multithtreading), 
so we will run the program many times so as to check if the code works for all of them). The test files are present in tests folder which has to be run one by one to check if the code works for all the possibilities.
```
tmtest n <test_file_name>
```
OR run this command 
```
./zgt_test ../test-files/<test_file_name>
```
## Running project on Windows

For running this project on windows, you need to make changes in the makefile to point it to the right location
(change '/' to '\\'). 