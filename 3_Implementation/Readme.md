# Here are the below steps to run the code
* For Running and Building the code
     * Type make run in terminal
* For Running the Building tests
     * Type make run_test in terminal
* For static analysis
     * Type make static_analysis in terminal
* For dynamic analysis
     * Type make dynamic_analysis in terminal
* For code coverage
     * Type make coverage in terminal
* For cleaning
     * Type make clean in terminal
# USAGE OF PREPROCESSOR/POINTERS/FUNCTION POINTERS/STRUCT/TYPE DEF
## Preprocessor:
The C preprocessor is a macro processor that is used automatically by the C compiler to transform your program before actual compilation. It is called a macro processor because it allows you to define macros, which are brief abbreviations for longer constructs.

### The C preprocessor provides four separate facilities that you can use as you see fit:
Inclusion of header files. These are files of declarations that can be substituted into your program. Macro expansion. You can define macros, which are abbreviations for arbitrary fragments of C code, and then the C preprocessor will replace the macros with their definitions throughout the program. Conditional compilation. Using special preprocessing directives, you can include or exclude parts of the program according to various conditions. Line control. If you use a program to combine or rearrange source files into an intermediate file which is then compiled, you can use line control to inform the compiler of where each source line originally came from.

## Pointers:
Pointers: The Pointer in C, is a variable that stores address of another variable. A pointer can also be used to refer to another pointer function. A pointer can be incremented/decremented, i.e., to point to the next/ previous memory location. The purpose of pointer is to save memory space and achieve faster execution time. Like variables, pointers in C programming have to be declared before they can be used in your program. Pointers can be named anything you want as long as they obey C’s naming rules. A pointer declaration has the following form.

syntax: data_type * pointer_variable_name;
Types of Pointers in C: 1.Null Pointer 2.Void Pointer 3.Wild pointer 4.Dangling pointer

## funtion pointer:
In the C function pointer is used to resolve the run time-binding. A function pointer is a pointer that stores the address of the function and invokes the function whenever required. In C, we can use function pointers to avoid code redundancy.

Unlike normal pointers, a function pointer points to code, not data. Typically a function pointer stores the start of executable code.
Unlike normal pointers, we do not allocate de-allocate memory using function pointers.
## Struct:
A structure is a key word that create user defined data type in C. A structure creates a data type that can be used to group items of possibly different types into a single type.

‘struct’ keyword is used to create a structure.

A structure variable can either be declared with structure declaration or as a separate declaration like basic types.Structure members cannot be initialized with declaration.

Structure members can be initialized using curly braces ‘{}’. For example, following is a valid initialization. Structure members are accessed using dot (.) operator.

## type def:
typedef, which you can use to give a type a new name. Following is an example to define a term BYTE for one-byte numbers.After this type definition, the identifier BYTE can be used as an abbreviation for the type unsigned char

By convention, uppercase letters are used for these definitions to remind the user that the type name is really a symbolic abbreviation, but you can use lowercase.

You can use typedef to give a name to your user defined data types as well. For example, you can use typedef with structure to define a new data type and then use that data type to define structure variables directly

Syntax: typedef data_type new_name
# Conditional Statements:-
The Conditional Statements help you to make a decision based on certain conditions.
## If Statement:
The single if statement is used to execute the block of code if a condition is true.
#### Syntax
   if(expression)
   {
      //code to be executed
   }
## If-else Statement:
This statement is used to execute the code if condition is true or false.It is also called two-way selection statement.
#### Syntax
      if(exp)
      {
       //statements
      }
      else
      {
       //statements
      }
## Nested If-else Statement:
This statement is used when a program requires more than one test expression.It is also called a multi-way selection statement.
#### Syntax
     if(exp)
     {
      if(exp1)
      {
       statements---1;
      }
      else
      {
       statements---2;
      }
     }
     else
     {
      statements----3;
     }
## If..else if ladder:
Which is used to execute one code from multiple conditions.
  #### Syntax
        if(cond1)
        {
          //statements
        }
        else if(cond2)
        {
          //statements
        }
        else if(cond3)
        {
         //statements
        }
        else
        {
         //statements
        }
## Switch:
Switch case statement evaluates a given expression and based on the evaluated value,it executes the statements associated with it.The switch statement,Which is used to perform different actions based on different conditions.
* Switch case statements follow a selection-control mechanism and allow a value to change control of execution.
* They are a substitute for long if statements that compare a variable to several integral values.
* The switch statement is a multiway branch statement. It provides an easy way to dispatch execution to different parts of code based on the value of the expression.
#### Syntax

switch (n)
{
    case 1: // code to be executed if n = 1;
        break;
    case 2: // code to be executed if n = 2;
        break;
    default: // code to be executed if n doesn't match any cases
}
# File Handling Functions
## fopen():
The fopen function opens a file called filename and associates it to stream.The fopen function clears all error and EOF indictors for the stream.The fopen() function also creates a new file.
 #### Syntax
          FILE*fopen(const char *file_name,const char *mode_of_operation);
 ## fclose():
 The fclose() function closes a stream pointed to by stream.This function deletes all buffers that are associated with the stream before closing it.Whwn it closes the stream ,the function releases any buffers that the system reserved.When a binary stream is closed,the last record in the file is padded with null charactrers(\0) to the end of the record.
 #### Syntax
      int fclose(FILE *stream);
 
