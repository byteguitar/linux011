## 隐式规则
  .c.s:
    $(CC) $(CFLAGS) \
	  -nostdinc -Iinclude -S -o $*.s $<
    
      这是make 老式的隐式后缀规则。
     该行指示make 利用下面的命令将所有的.c 文件编译生成.s 汇编程序。':'表示下面是该规则的命令 **注意是下一行命令**
      如下是运用规则
      boot/head.o: boot/head.s
