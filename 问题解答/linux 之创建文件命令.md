1、vi

vi 1.txt 会直接创建并打开一个文件1.txt

2、touch

touch的作用是更改一个文件或目录的时间。touch 2.txt 如果2.txt不存在，则创建空文件2.txt

3、echo 

echo “abcd” > 3.txt 可以直接创建文件3.txt并将abcd写入。

4、less 、more 、cat 

三者都是将文件内容输出到标准输出，其中less和more可以分页显示，cat是显示全部。

三者可以根据已经存在的文件创建新的文件。假设已经存在文件1.txt。

cat 1.txt > 2.txt

less 1.txt > 3.txt

more 1.txt > 4.txt

此时创建的文件内容都和1.txt中文件内容相同。