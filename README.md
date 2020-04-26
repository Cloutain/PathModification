# PathModification
Process path modification x64

作者：猪会被杀掉

支持 x64下（win7 ~ win10 all） 对x64进程的路径修改

另外一种实现方法就是 傀儡进程

KMAX_PATH = 300

PsGetProcesIdBitByName->这个函数的功能是获取指定位数的进程id（第二个参数控制是x86还是x64进程） 在内部判断了进程是多少位的 这个功能只针对64位进程 你直接实现一个函数 获取64位的进程id就行了
