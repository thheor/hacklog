## Bandit Level 2 -> 3

Level Goal

The password for the next level is stored in a file called --spaces in this filename-- located in the home directory
Commands you may need to solve this level

`ls , cd , cat , file , du , find`

Helpful Reading Material

[Google Search for “spaces in filename”](https://www.google.com/search?q=spaces+in+filename)

## Spaces in Filename

Spaces in Unix filename create challenges for users working in terminal. The command line treats whitespace as argument separators, which causes errors when we reference files with gaps in their name.

To handle this challenges, we can use **quotation marks** around the filename or use backslashes (`\`) before each spaces.

## Solution

```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org

ls -als

cat --spaces\ in\ this\ filename-- # or
cat -- '--spaces in this filename--'
```

Then you must the password for the next level:

```bash
7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
```
