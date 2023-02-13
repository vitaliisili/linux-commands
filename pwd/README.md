# **Command Line Basic**
 *There are some basic things to understand about command line that will help you effectively harness this powerful tool.*

 About `$` and `#` characters:
 
 - `$` character means you are a normal user with limited rights
 - `#` character means you are a super user with all rights.



## **`pwd`**  Command

*- Print the name of the current working directory.*

### Syntax:
```
pwd: pwd [-LP]

```

#### Options:
   
   `-L` : print the value of $PWD if it names the current working
    		directory.

`-P` :   print the value of `$PWD` if it names the current working
    		directory.

*By default, `pwd`   behaves as if  `-L` were specified.*
  

  ##### **Short and Long parameters**:
  ```
  Short parameters are the most common used. Usually just one letter preceded by a dash(-).For example: -l, -a.
  Long parameters are usually several characters preceded by double dashes (--).For example: --all, --version .