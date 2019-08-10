1. In __C__, _main_ function can have return type as __void__ while in __C++__, _main_ function cannot have __void__ as well as __long__ as return type.

2. If you don't specify any return value then it is by default __int__ in C/C++ .

3. __Compiling__ refers to conversion of source code into object code.  This step doesn't create anything the user can actually run. Instead, the compiler merely produces the machine language instructions that correspond to the source code file that was compiled.

4. __Linking__ refers to the creation of a single executable file from multiple object files. During compilation, if the compiler could not find the definition for a particular function, it would just assume that the function was defined in another file. The linker, on the other hand, may look at multiple files and try to find references for the functions that weren't mentioned. If not found, then linker will complain.

5. A __preprocessor__ is a program the process the source code before it passes through the compiler. Preprocessor operates under the control of __Preprocessor Directives__ . Example of Preprocessor Directives are #include, #define, #undef, #ifdef, etc.

6. __Prefix operators__ like __++a__ or __--a__ first increments the value and the return the incremented value. Whereas, __Postfix operators__ like __a++__ or __a--__ first returns the original value and then increments it.

7. __getchar()__ keeps on reading the input until enter key is pressed.  
__getch()__ reads only a single character and returns it immediately.  
__getche()__ also reads only a single character but it returns as well as prints the character which was read.

8. We cannot perform arithmetic operations between two pointers.

9. When we increment a pointer, it's value is changed by the length of data type that it points to. This length is known as __scale factor__.

10. A __void pointer__ can be used to point to variables of any data type.

11. In C, dynamic memory is allocated from the heap using some standard library functions. The two key dynamic memory functions are __malloc()__ and __free()__.  These functions are present in __stdlib.h__ header file.  
C++ supports these functions and also has two operators **new** and **delete** that perform the task of allocating and freeing the memory in a better and easier way.

12. The __malloc()__ function takes a single parameter, which is the size of the requested memory area in bytes. It returns a pointer to the allocated memory. If the allocation fails, it returns NULL.  
Example:  
	```
	int *pointer;  
	pointer = malloc(10 * sizeof(int));  
	```

13. The __free()__ function takes the pointer returned by malloc() and de-allocates the memory. No indication of success or failure is returned.  
Example:  
`free(pointer);`

14. There's one more function which is used to allocate memory dynamically.  
The __calloc()__ function does basically the same job as malloc(), except that it takes two parameters – the number of array elements and the size of each element – instead of a single parameter (which is the product of these two values). The allocated memory is also initialized to zeros.
Example:
`pointer = calloc(num_of_elements, sizeof_element); `

15. To allocate memory of any data type using __new__ operator, the syntax is:
`pointer_variable = new data-type;`  
__For arrays:__
`pointer_variable_2 = new data-type[];`

16. To deallocate memory pointed by pointer_variable using __delete__ operator, the syntax is:  
`delete pointer_variable;`  
__For arrays:__
`delete []pointer_variable_2;`

17. The operator `<<` is called __insertion__ or __put to__ operator. Whereas, the operator `>>` is called __extraction__ or __get from__ operator.

18. When we declare a member of a class as __static__ it means no matter how many objects of the class are created, there is only one copy of the static member and this one copy is shareable among all the objects.  
All static data is initialized to __zero__ when the first object is created, if no other initialization is present.

19. If a function is __static__ then there's __no need to create object__ for calling that function. Also a __static function__ can only access __static data member__.

20. __this__ refers to the __invoking object__. Only member functions have a __this__ pointer.

21. __friend__ functions should be declared inside the class definition, but they will __not__ be member functions of that class.  

22. __friend__ function has the right to access __all members__(public, private, protected) of the class but since it is not member function of that class, it __cannot access the members directly__. Instead it uses another object of that class to access members.

23. __friend__ function takes object of class as argument. Also, __friend__ functions are called normally without  any object.

24. Example of __friend__ function:  
	```
	class A
	{
	    int num;
	    public:
	    void get()
	    {
	        cout << "enter the number:";
	        cin >> num;
	    }
	    friend void showTable(A obj);
	};
	void showTable(A obj)
	{
	    int i;
	    for(i=1;i<11;i++)
	        cout << obj.num*i << endl;		//accessing 'num' through obj
	}
	int main()
	{
	    A t1;
	    t1.get();
	    showTable(t1);
	}
	``` 

25. We can also define a __friend__ class of another class.

26. All variables declared inside the function will take up memory from the __stack__. Whereas when we dynamically allocate memory, it is allocated on __heap__.