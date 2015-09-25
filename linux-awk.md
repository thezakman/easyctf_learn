# Awk

AWK is an interpreted programming language designed for text processing and typically used as a data extraction and reporting tool. It is a standard feature of most Unix-like operating systems.

For example, to search the word "hello" in "test.txt":

```bash
awk /hello/ test.txt
```
    
You can also search in multiple files, or use the wild card, the asterisk `*`, to search all files in a directory.

```bash
awk /hello/ test1.txt test2.txt test3.txt
```
    
or

```bash
awk /hello/ *
```
    
Just like with grep, there are several different options you can apply to awk to make it more or less specific.

## '{print $1}'
This option will print only the first word searched. This means if the file was test.txt, "world" would be printed. You can use any digit or 0 to print the full text in the files specified.

```bash
grep -i "key" *
```
    
## -l
This option lists only the file name that contains the word or phrase being searched.

```bash
grep -l "hello" *
```
    
## -r
Similar to cat, this option recursively searches the word or phrase in all sub-directories.
    
```bash
grep -r "hello" *
```
    
