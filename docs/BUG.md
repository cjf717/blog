# EMFILE 错误
- Error: EMFILE, too many open files
虽然 Node.js 有非阻塞 I/O，同步 I/O 的数量仍被系统所限制，在生成大量静态文件的时候，您可能会碰到 EMFILE 错误，您可以尝试提高同步 I/O 的限制数量来解决此问题。

官网中只介绍了linux的做法，没有windows系统下的操作。当文件过多时，加载需要时间也很长。
