# Step01Homework

Homework For Step 01

### 找到在 Ubuntu 系统中可以用于计算文件内容 MD5 值的命令过于简单，暂无参考答案

```
md5sum
```

### 找到在 Ubuntu 系统中可以用于比较两个文件的内容的差异的命令过于简单，暂无参考答案

```
diff
```

### 实现一个名为 odd-or-even 的 Bash function，可以用来判断给其提供的第一个参数是奇数还是偶数，奇数时输出 odd，偶数时输出 even

```
$ vim ~/bin/odd-or-even

#!/bin/bash

NUM=$@

if [[ "" == "$NUM" ]]
then
        echo no input
else
if [[ 0 == `expr $NUM % 2` ]]
then
        echo even
else
        echo odd
fi

fi

chmod -x ~/bin/odd-or-even

```

### 实现一个名为 next 的脚本，当在 CLI 里执行 $ next （$为提示符，不需要输入）时就返回一个整数，第一次返回 1，每执行一次加 1 参考答案还未准备好 

```
$ vi ~/bin/next

#!/bin/bash

if [[ ! -f "/tmp/value.dat" ]]
then
        NUMCOUNTER=0
else
        NUMCOUNTER=`cat /tmp/value.dat`
fi


NUMCOUNTER=$((NUMCOUNTER + 1))
echo $NUMCOUNTER
echo "$NUMCOUNTER" > /tmp/value.dat

chmod +x ~/bin/next

```

### 


