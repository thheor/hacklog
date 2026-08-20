## Bandit Level 1 -> 2

Level Goal

The password for the next level is stored in a file called - located in the home directory

Commands you may need to solve this level

`ls , cd , cat , file , du , find`
Helpful Reading Material

[Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
[Advanced Bash-scripting Guide - Chapter 3 - Special Characters](https://linux.die.net/abs-guide/special-chars.html)

## Dashed Filename

A dashed filename is a file name that begins with a dash or hyphen (e.g., `-filename`, or just `-`). This name is still valid but will leads to unique challenge because the command-line interface natively interprets a dash as a command option or flag rather than a file argument.

## Solution

To solve the challenge of the dashed filename while using a command-line interface, like `cat`, we can use `cat ./-filename`.

```bash
ssh -p 2220 bandit1@bandit.labs.overthewire.org

ls -als

cat ./-
```

By using those command, we must get the following output:

```bash
PK8fYLZg2hnHSz83plBL1iEPKdD3QToB
```

This is the password that we can use to login into the next level.

### Explanation

`ls -als`

`-l` is used to display the detailed information.
`-a` is used to display all files including hidden files.
`-s` is used to display the allocated size of each file in blocks.
