## Bandit Level 4 -> 5

Level Goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.
Commands you may need to solve this level

`ls, cd, cat, file, du, find`

## Solutions

```bash
ls -als

cd inhere
ls -als
file ./* # you will get the file information including the type of data stored in each file
cat ./-file07 # because only -file07 that contains ASCII text
```
