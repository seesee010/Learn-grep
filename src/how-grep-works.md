# Here is how grep works

Here is a quick guide about what `grep` is and how you can use it.

## TOC

<!-- TOC -->

- [Here is how grep works](#here-is-how-grep-works)
    - [TOC](#toc)
    - [General use of grep](#general-use-of-grep)
    - [Attributes](#attributes)
        - [-i - case insensitive](#-i---case-insensitive)
        - [-n - show lineNum](#-n---show-linenum)
        - [-v - show everything else](#-v---show-everything-else)
        - [-c - count matches](#-c---count-matches)
        - [-r - whole dir](#-r---whole-dir)

<!-- /TOC -->

## General use of grep

Grep is a cmd to find text in a certain file!

```bash
grep "whatIwantToFind" path/to/file.txt
```

Here is the code if you wanna try it:

```bash
grep "Hello" src/test.txt
```

> [!NOTE]
> This would print out:
>
> Hello World
> Hello I am seesee010


## Attributes


### `-i` - case insensitive

```bash
grep -i "Hello" src/test.txt
```

> [!NOTE]
> This will print out 
> Hello and HELLO or any other case

### `-n` - show lineNum

```bash
grep -n "Hello" src/test.txt
```

> [!NOTE]
> This will also print out 
> the corresponding line number

### `-v` - show everything else

```bash
grep -v "Hello" src/test.txt
```

> [!NOTE]
> This will show everything what is not matching
> (inverted search)

### `-c` - count matches

```bash
grep -c "Hello" src/test.txt
```

> [!NOTE]
> This shows how many lines contain the pattern.

### `-r` - whole dir

```bash
grep -r "Hello" src/
```

> [!NOTE]
> Seach through a whole directory.