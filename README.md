# ClangDirectivesRecord
Clang Directives Record

```C++
// Declare passing Directives parameters to the linker
#pragma comment(linker, "/SECTION:.jmb,RWESP")

// Make parameters inside '.jmb' section
#pragma data_seg(push, label, ".jmb")
int g_x = 3;
#pragma data_seg(pop, label)

```

```C++
// Make 'myfunc' function inside '.virs' section
__declspec(code_seg(".virs"))
int myfunc();
```
