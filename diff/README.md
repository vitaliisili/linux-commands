# diff

*The `diff` command line tool is used to compare the contents of two files line by line and display the differences.*

## Syntax

```bash
diff [option] file1 file2
```
where *file1* and *file2* can be either relative or absolute paths.

## Usage

Depending on the used options, `diff` can display the changes between files in different ways.
Lets assume we have two simple text files with the following content:
#### File1:
>Cat  
Dog  
Horse  
Duck  
Sheep  
#### File2:
>Cat  
Horse  
Cow  
Duck  
Sheep and Goats  

When calling diff without any options the output of `diff file1 file2` will look like this:

```bash
2d1
< Dog
3a3
> Cow
5c5
< Sheep
---
> Sheep and Goats
```

`diff` shows the changes with the syntax: `<original line> <type of change (a, d or c)> <changed line>`
So in this example we see that the first change is on line two of the original file and is deleting one line (`2d1`). Below that we see what was deleted (`< Dog`).
The next change added the word `Cow` to Line 3 (`3a3`). And finally, we changed line 5 from `Sheep` to `Sheep and Goats` - (`5c5`)

Different Options can modify the style of the output. For example, `-c` gives the output more context:
```bash
*** file1       2023-02-13 16:08:54.984539815 +0100
--- file2       2023-02-13 16:08:47.561091607 +0100
***************
*** 1,5 ****
  Cat
- Dog
  Horse
  Duck
! Sheep
--- 1,5 ----
  Cat
  Horse
+ Cow
  Duck
! Sheep and Goats
```

Here, deletions, insertions and modifications are indicated by `-`,`+` and `!`

Another option that might be easier to read for some is the unified output with `-u`:
```bash
--- file1       2023-02-13 16:08:54.984539815 +0100
+++ file2       2023-02-13 16:08:47.561091607 +0100
@@ -1,5 +1,5 @@
 Cat
-Dog
 Horse
+Cow
 Duck
-Sheep
+Sheep and Goats
```

There is also the possibility to show the differences side-by-side with `-y`:
```bash
Cat                                                             Cat
Dog                                                           <
Horse                                                           Horse
                                                              > Cow
Duck                                                            Duck
Sheep                                                         | Sheep and Goats
```
