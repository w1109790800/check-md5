# check-md5
> 这是一个便于自己写python程序的小工具 \
因为写python的时候，如果不用IDE(自己喜欢用Vim)，调试总要退出vim或者另开一个终端，但如果另开一个终端还要用鼠标。\
所以就有了这个小工具
## 原理如下
 首先，在程序运行之初就写入一部分内容，便于以后继续写
 自动写入内容如下
![](https://raw.githubusercontent.com/w1109790800/check-md5/master/2.jpg)
 ```python
 import os 
import math 
import time 
 
def main():
    print("Hello World")



if __name__ == "__main__":
    main()
```
 之后获取文件md5，并且每5秒重新获取一次。
 如果文件变化，那么md5必然变化，这样就可以自动执行
```python
 Python XXX.py
```
这个命令了
![](https://raw.githubusercontent.com/w1109790800/check-md5/master/1.jpg)