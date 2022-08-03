# c_lang_linux_tips_&_tricks

# Minimal Linux Command Line C Program Compile & Run

#### Assuming you have a source code file,  e.g.  "source_file_name.c"
```
#include<stdio.h>
int main()
{
	printf("Hello World");
	return 0;
}
```

#### Step 1: Compile
```
$ gcc -o executable_file_name source_file_name.c
```
#### Step 2: Run
```
$ ./executable_file_name 
```



# running c executable files in linux
https://vitux.com/how-to-execute-bin-and-run-files-in-ubuntu/

### Step 1: setup to be able to run the file on your system
```
$ sudo chmod +x ./FILENAME.run
or
$ sudo chmod +x ./FILENAME.exe
```

### Step 2: run the file
```
$ ./FILENAME.run
or
$ ./FILENAME.exe
```


# arguments
https://www.geeksforgeeks.org/command-line-arguments-in-c-cpp/ 

