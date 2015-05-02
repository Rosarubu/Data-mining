```
cut -f1 file| sort -u | wc -l # file no of unique row
awk -F ',' '{print $1}' file| wc -l #split file using , then find no of row in column 1 
awk -F ',' '{print $1}' file| sort -u | wc -l #split file using , then find no of unique row in column 1
```

[^M delete] (http://blog.csdn.net/zhangguangyi888/article/details/8159601)      
在Vim中解决这个问题，很简单，在Vim中利用替换功能就可以将“^M”都删掉，键入如下替换命令行：
:%s/^M//g
注意：
上述命令行中的“^M”符，不是“^”再加上“M”，而是由“Ctrl+v”、“Ctrl+M”键生成的，或者Ctrl+v，再按回车。
或者使用这个命令：
:% s/r//g
