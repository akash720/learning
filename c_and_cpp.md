1. In __C__, _main_ function can have return type as __void__ while in __C++__, _main_ function cannot have __void__ as well as __long__ as return type.
2. If you don't specify any return value then it is by default __int__ in C/C++ .
3. __Compiling__ refers to conversion of source code into object code.  This step doesn't create anything the user can actually run. Instead, the compiler merely produces the machine language instructions that correspond to the source code file that was compiled.
4. __Linking__ refers to the creation of a single executable file from multiple object files. During compilation, if the compiler could not find the definition for a particular function, it would just assume that the function was defined in another file. The linker, on the other hand, may look at multiple files and try to find references for the functions that weren't mentioned. If not found, then linker will complain.
5. A __preprocessor__ is a program the process the source code before it passes through the compiler. Preprocessor operates under the control of __Preprocessor Directives__ . Example of Preprocessor Directives are #include, #define, #undef, #ifdef, etc.
6. __Prefix operators__ like __++a__ or __--a__ first increments the value and the return the incremented value. Whereas, __Postfix operators__ like __a++__ or __a--__ first returns the original value and then increments it.
7. __getchar()__ keeps on reading the input until enter key is pressed.  
__getch()__ reads only a single character and returns it immediately.  
__getche()__ also reads only a single character but it returns as well as prints the character which is read.
8. We cannot perform arithmetic operations between two pointers.
9. When we increment a pointer, it's value is changed by the length of data type that it points to. This length is known as __scale factor__.
10. A __void pointer__ can be used to point to variables of any data type.
11. In C, dynamic memory is allocated from the heap using some standard library functions. The two key dynamic memory functions are malloc() and free().  
The __malloc()__ function takes a single parameter, which is the size of the requested memory area in bytes. It returns a pointer to the allocated memory. If the allocation fails, it returns NULL.  
Example:  
	```
	int *pointer;  
	pointer = malloc(10 * sizeof(int));  
	```
	The __free()__ function takes the pointer returned by malloc() and de-allocates the memory. No indication of success or failure is returned.  
	Example:  
	`free(pointer);`