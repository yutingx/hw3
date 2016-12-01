## Edit distance
### By Yigan Zhang(18324490) & Yuting Xue(31323149)
  The program would read input from a file. The output is a list of edit distance and their corresponding sequence of transformation operations.
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
  Find `fpt`in edit.cpp (line 142)
  This is where you can change your output's name.
  ```
  FILE *fpt = fopen("output1.txt", "w");
  ```
####Change inputs
Find `fp`in main function in edit.cpp (line 234)
  This is where you can change your intput's name.
  ```
  FILE*fp = fopen("input1.txt", "r");
  ```
### my little SAMPLE!
  I wrote a sample at the bottom of program, you can test it first if you are interest.

### For question 1
  You need to change input strings to be `electrical engineering,`and `computer science.`. 
  First, you need to add `/* `before `int main()` and add another `*/` at the end of `return 0}` of paragraph of `INPUT FILES`.
  Then, release 
  ```
 int main()
{ 
  char str1[]="electrical engineering,";
  char str2[]="computer science.";
		
    int edit=0;
    edit = edit_distance(str1, str2);
		
    return 0;
}

  ```
  by removing `/*` and `*/`before and after paragraph of `For question 1`.
  Finally, run the program you will see the output of question 1.
### For question 2
  You need to release `INPUT FILES` paragraph and keep annotation for both `For question 1` and `my little SAMPLE!`.
  
  If you don't want to see corresponding sequence of transformation operations, you need to add `//` before line 147, 148, 153, 154, and also add `/* and */` for paragraph below:
```
    k--;
    int m=k;
    for(int i=0;i<m;i++)
    ......
  
    //printf("right:%d,insert:%d,delete:%d,substitute:%d\n",right,insert,delet,substit);*/
```
  Then, By changing `input1.txt` to `input2.txt`and`input3.txt`, you will get result of those three both on your teminal and output files.

### For question 3
    Besides two array of x, y, you need two more array str1 and str2.
    For example, when edit 'lgo' to 'algo' in x and y, you need to insert 'a' in an empty array str1, paste x to an empty array str2. And first print str1, then str2, finish insert.
    When edit 'algo' to 'lgo' in x, y, paste letter after 'a' in x to an empty array str1, print str1, finish delete.
    when edit 'ago' to 'lgo' in x,y, add letter 'l' to array str1, paste letter after 'a' in x to str2, print str1 and str2, finish replace.
    By doing this, you can implement in O(1) time.

  
  Thanks for reading :blush:
  
    
