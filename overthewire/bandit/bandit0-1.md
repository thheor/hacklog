## Bandit Level 0 → Level 1

Level Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into **bandit1** using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

Commands you may need to solve this level

```bash
ls , cd , cat , file , du , find
```

TIP: Create a file for notes and passwords on your local machine!

Passwords for levels are **not saved automatically**. If you do not save them yourself, you will need to start over from bandit0.

Passwords also occasionally change. It is recommended to take notes on how to solve each challenge. As levels get more challenging, detailed notes are useful to return to where you left off, reference for later problems, or help others after you’ve completed the challenge.

## Solutions

Open your terminal and type this command:

```bash
ssh -p 2220 -l bandit0 bandit.labs.overthewire.org # or you can use
ssh -p 2220 bandit0@bandit.labs.overthewire.org
```

Then use this command to concatenate readme file and get the password for the next level:

```bash
cat readme
```

The output should looks like this:

```bash
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
```

You can use that password to login to the next level.
To exit the ssh, just type `exit` in the terminal.

### Explanation

Explanation while using ssh to login into remote machine.
`-p` is used to specified the port of the machine that we want to log in.
`-l` is used to specified the username of the machine.
