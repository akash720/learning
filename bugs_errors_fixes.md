# 1. MinGW issue with conda python
If you are facing the issue "cannot find -lvcruntime140" while building from setup.py file then follow the steps below:

1. First install the libpython and toolchain by using the following command:
`conda install libpython m2w64-toolchain`

2. Open distutils.cfg file present in `<Path to Anaconda Installation>\Lib\distutils\` . If it is not there, create one. Type the following in the file:
```
[build]
compiler = mingw32
```
3. Save and close the file.

4. Open the file cygwinccompiler.py which is located in <Path to Anaconda Installation>\Lib\distutils\ and comment the following:
* On line 158 to 161
 ```
	else:
            # Include the appropriate MSVC runtime library if Python was built
            # with MSVC 7.0 or later.
            self.dll_libraries = get_msvcr()
```

* On line 327
`self.dll_libraries = get_msvcr()`

What commenting these lines does is to tell cygwin compiler to not look for visual studio.

5. Save the file cygwinccompiler.py

6. Make sure that MinGW is in System Environment Path (below paths):
```
<MinGW installation path>\bin
<MinGW installation path>\msys\1.0\bin
```