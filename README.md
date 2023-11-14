# EX 5b: Command-line-arguments-to-count-word
## DATE: 10.10.23
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### STEP 1:
Import sys module to use command line arguments

### Step 2:
Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument

### Step 3:
Iterate the content of the file using for loop.

### Step 4:
Split the contents into each line using .split() function.

### Step 5:
Iterate the list of lines and increment the value of variable (word) each time.

### Step 6:
Run the program by giving "python prgm.py EX12.txt" on the terminal.
## PROGRAM:
```
# Ex5b-command line arguments(word count)
# Program Developed By: DIVYA.A
# Register Number: 212222230034
import sys
count={}
with open('/content/file1.txt','r') as f:
  for line in f:
    for word in line.split():
      if word not in count:
        count[word]=1
      else:
        count[word]+=1
print(count)
f.close()
```
## FILE:
![Exp 5b(1)](https://github.com/Divya110205/command-line-arguments-to-count-word/assets/119404855/78906e8d-578c-4d2c-89c1-8c7d965f741a)

## OUTPUT:
![Exp 5b(2)](https://github.com/Divya110205/command-line-arguments-to-count-word/assets/119404855/be3995f5-41a5-4b9a-9d68-f280c8a5d421)

## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
