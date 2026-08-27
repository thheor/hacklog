## Bandit Level 5 -> 6

Level Goal

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

`human-readable
1033 bytes in size
not executable`

Commands you may need to solve this level

`ls, cd, cat, file, du, find`

## Solution

```bash
cd inhere

find . -type f -size 1033c
cat ./maybehere07/.file2
```
