# glog
在[golang/glog](https://github.com/golang/glog) 的基础上做了一些修改。

## 修改的地方:
1. 增加每天切割日志文件的功能,程序运行时指定 --dailyRolling=true参数即可
2. 将默认的刷新缓冲区时间由20s改为5s

//假设编译后的可执行程序名为demo,运行时指定log_dir参数将日志文件保存到特定的目录
// ./demo --log_dir=./log --dailyRolling=true 
