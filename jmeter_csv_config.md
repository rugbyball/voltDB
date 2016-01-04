

ref: http://lijingshou.iteye.com/blog/2047613

以下是CSV Data Set Config各个参数的简要说明:<br />
FileName:即同目录下csv文件的名称<br />
File Encoding: 默认为ANSI<br />
Varible Names: 定义文本文件中的参数名,参数之间逗号分隔.定义后可在脚本在以Shell变量的同样的方式引用<br />
Allow Quoated data: 双引号相关<br />
Recycle on EOF: 设置为True后,允许循环取值<br />
Stop Thread on EOF: 当Recycle on EOF为false并且Stop Thread on EOF为true,则读完csv文件中的记录后,停止运行<br />
Sharing Mode: 设置是否线程共享<br />
