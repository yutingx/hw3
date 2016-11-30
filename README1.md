## Edit distance
### By Yigan Zhang & Yuting Xue
  The program would read input from a file. The output is a list of edit distance and their corresponding sequence of transformation
operations.
### How to use it?
  Tap in teminal
```
cd hw4
make
./edit
```
  You will see the output both in a file and your teminal. 
### How to modify it?
####Change outputs
  Find `fpt`in edit.cpp
  This is where you can change your output's name.
  ```
  FILE *fpt = fopen("output1.txt", "w");
  ```
####Change inputs
Find `fp`in main function in edit.cpp.
  This is where you can change your intput's name.
  ```
  FILE*fp = fopen("input1.txt", "r");
  ```
### For question 1
  You need to change input strings to be `electrical engineering,`and `computer science.`. 
  First, you need to add `/* `before `FILE` in main() and add another `*/` at the end of `fclose(fp);`.
  Then, release 
  ```
  char str1[]="electrical engineering,";
  char str2[]="computer science.";
  ```
  by removing `//`before them.
  Finally, run the program you will see the output.
### For question2
  Just keep the original file and run it, you will get result of input1.txt.
  By changing `input1.txt` to `input2.txt`and`input3.txt`, you will get result of those two.

  
  Thanks for reading :blush:
  
    
