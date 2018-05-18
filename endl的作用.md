## endl的作用
endl的作用是换行可以插入到输出流中，效果为在输出结果中插入换行符'\n'。

要直接使用endl，需要使用std名空间，即使用：
`using namespace std;`
否则需要使用`std::endl`
以标准输出流cout为例：

```
cout << "this is a test string" <<endl;
```
的效果就是输出`this is a test string`后换行。
用于文件输出流或字符串输出流时用法类似。

## `system("pause")` 与 `cin.get()`

在程序中，使用 `system("pause")` 暂停程序的运行。但是这样做，开销太大。我们使用 `cin.get()` 代替。
```
    #include <iostream>
    using namespace std;

    int main()
    {
        cout << "hello, 卧槽" << endl;
        system("pause");  //  使用: cin.get(); 代替

        return 0;
    }
```

## C++入门
```
    #include <iostream>
    using namespace std;

    int main()
    {
        cout << "你好啊，世界";
        return 0;
    }
```
下面来讲解下上面这段最简单的程序:
* C++语言定义了一些头文件，这些头文件包含了程序中必须的或有用的信息。上面这段程序中，包含了头文件`<iostream>`。
* 下一行 `using namespace std;` 告诉编译器使用了std 命名空间。
* 下一行 `int main()` 是主函数，程序冲这里开始执行。
* 下一行 `cout << "你好啊，世界";` 会在控制台上打印出 '你好啊，世界'。
* 下一行 `return 0;` 终止 main() 函数。并向调用进程返回值0。

## C++中的分号 & 块
在C++中，分号是语句结束符。也就是说，每个语句必须以分号结束。它表明一个逻辑实体的结束。

分号必须写，否则会报错。
## C++ 注释
C++中的注释和js里的一样。

## 预编译指令与分号
在C++中，除函数，及预编译指令外，其它的语句或代码段结尾都必须要加分号。
其中预编译指令是指，以#开头的语句。常见的有，#include ,#define, #ifdef, #if, #elif, #else，#endif等。