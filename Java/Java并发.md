#### 线程和进程

进程简单理解就是运行中的程序，是程序的一次运行过程。

进程的状态：Running、Blocked、Ready

进程对内存的访问是互相隔离的，因此进程进行上下文互相切换的时候有较大的开销（如切换页表等）

线程是比线程更小的执行单位，用户级线程对操作系统是透明的，线程共享进程的堆和方法区资源，但是每个线程都有自己的**程序计数器、虚拟机栈和本地方法栈**，线程进行上下文切换时开销比较小

为什么程序计数器、虚拟机栈和本地方法栈是私有的

并发与并行：并行——同时运行，并发——交替运行

同步和异步：同步——等待返回结果，异步——不必等待结果，直接返回

#### 线程上下文切换

线程在执行过程中会有自己的运行条件和状态（也称上下文），如上文提到的程序计数器、栈信息等。当发生以下情况时，线程会从占用CPU状态退出。

* 主动让出CPU，比如调用了`sleep()`,`wait()`等；
* 时间片用完，操作系统要防止进程或线程饥饿；
* 调用了阻塞类型的系统中断，比如请求IO，线程被阻塞；
* 被终止或结束运行

这其中前三种都会发生线程切换，也即保存当前线程的上下文，留待之后使用，加载下一个将要占用CPU的线程的上下文。

#### 线程死锁

#### JMM（Java内存模型）

#### volatile关键字

在Java中，`volatile`关键字可以保证变量的可见性，如何我们将变量声明为`volatile`，这就知识JVM，这个变量是共享且不稳定的，每次使用它都到主存中进行读取。

`volatile`关键字能保证数据的可见性，但不能保证数据的原子性。`synchronized`关键字两者都能保证。

