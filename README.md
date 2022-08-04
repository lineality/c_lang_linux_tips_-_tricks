# c_lang_linux_tips_&_tricks

#  Compile & Run: minimal linux terminal process
using gcc to compile a C language program

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


# input arguments
```
$ ./FILENAME.exe ARGUMENT_1 ARGUMENT_2 ETC
```

```
#include <stdio.h>

int main( int argc, char *argv[] )  {

    // you will use this to store an input
    int input_a;
    // you will use this to store the calculated number of added inputs
    int number_of_added_inputs;
 
    // calculate the number of added inputs
    number_of_added_inputs = argc - 1;
 
    // print the total number of inputs
    printf("number 'o added inputs: %d\n", number_of_added_inputs);

    // print each input and its number
    for (int i = 0; i < argc; ++i){
        // print its number 
        printf("%d is ", i);
        // print each input 
        printf("'%s'\n", argv[i]);
        }

    // ask user to type in a number:
    printf("Enter an integer\n");
    // read in the user input
    scanf("%d", &input_a);
    
    // read back the input
    printf("You typed in this, yes?  %d\n", input_a);
    
// Finish: OK!
return 0;
}

```

#### see: 
- https://www.tutorialspoint.com/cprogramming/c_command_line_arguments.htm
- https://www.geeksforgeeks.org/command-line-arguments-in-c-cpp/ 
- https://www.programmingsimplified.com/c/program/print-integer 
