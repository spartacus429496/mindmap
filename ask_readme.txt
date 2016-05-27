1.linux src tree 
1.1 ldd3 discription
1.2 ldd3 hello.c Makefile


2. gcc search header files setting?

4. linux userspace and kernel space data exchange 
每个进程有各自的私有用户空间（0～3G），这个空间对系统中的其他进程是不可见的。最高的1GB字节虚拟内核空间则为所有进程以及内核所共享


进程的虚拟地址在内核中通过三级页表到达物理地址。
而内核的虚拟地址在NORMAL部分算是逻辑地址只是线性的映射。
这两者有什么关系么？或者说内核态为什么还要有虚拟地址存在？
内核态为什么还要有虚拟地址存在?
why kernel needs virtual addressing?

用户态到内核态切换分析


驱动的全局变量，任何进程陷入内核态中均可以访问（因为内核页表是一致的）。
进程自己的全局变量，显然其它进程无法访问（因为使用的是不同的页表）。

在 Linux 下用户空间和内核空间数据交换的方式
3. interrupt can not blocking ?
reason ? 
 it has no reason to block
首先要参考http://linux.chinaunix.net/bbs/thread-902033-1-38.html 中4楼的发言。个人以为分析到位了。

再次，参考 http://lwn.net/Articles/302043/， 引入threaded_irq后，中断的下半部是可以休眠的了


4.cscope useage 
How to filter cscope output within Vim?


I am looking for a way to grep the output of cscope queries from Vim.

The following didn't work for me:

:cs f s symbol !grep pattern

It gave:

E259: no matches found for cscope query s symbol !grep pattern ...

P.S:
I know the redir method, I am looking for a simpler way to filter
output of ex command(s) through Unix commands.


5.bluetooth specification
specification of bluetooth system  profiles volume 2



6.life
100% pure new zealand video ads 2012


7.git 
git apply patch  trailing whitespace.

8.kernel moudle makefile 
src_tree
in ldd3 


9 .vim 
函数体跳转：
[[
]]
[]
][
{}

10.tongxin 
点到点 端到端 ppp

11.linux net driver net_device tcp ip statck sk_buffer , soket filesystem vfs


11. linux kref
12. singleton

13.nrf51 sdk ble multi tasking 

14. linux tcp数据包 怎么找到端口????
 tcp packet  frame , src port , dest port 


15. linux fasync , driver notify app 
dispatch messages   

16. drivers and filesystem i/O space

17.three important parts CPU , ram,  i/O devices  
ram主要是配置时序，在bootloader阶段驱动就加载好了  

18.grep
grep --exclude=*.cmd ckim * -r
