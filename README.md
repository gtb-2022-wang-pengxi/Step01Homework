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

