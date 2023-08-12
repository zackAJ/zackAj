# alias
step by step guide on how to set up a git bash alias with arguments globaly on Windows 

## Requirements

- Windows OS
- git installed
- git bash

---

## table of content

- [The Goal](#the-goal)
- [Command Setup](#command-setup)
- [Steps](#steps)

---

## The Goal
the goal of this example is to clone any repo from your GitHub profile,
you can apply the same logic and steps to setup any alias

Going from this :
```sh
git clone https://github.com/zackAJ/<projec-name>
```

To this :
```sh
clone <projec-name>
```

---

## Command Setup
in this example, I'm using my own GitHub profile URL: `https://github.com/zackAJ/`

don't forget to replace it with **your own URL**.
```sh
 alias clone='fn(){ git clone https://github.com/zackAJ/$1; } ; fn $1'
```
where:
- `clone` is the name of the alias, you can name this to anything you like.
- `$1` is going to be the argument that we pass to the function AKA our `repo name`.

once your command is ready copy it and follow these steps [Steps](#steps)

---

## Steps

1- go to `C:\Program Files\Git\etc\profile.d`

![image](https://github.com/zackAJ/allias/assets/101515566/a54502cf-7684-44cf-9594-7f3a28eb7f7b)

2- open `aliases.sh` with a text editor of choice `as an administrator`

3- paste your alias to add it to the list of global aliases and save

![image](https://github.com/zackAJ/allias/assets/101515566/b6da8fe1-918e-4974-bb76-6ae152d26310)

4- to check if the alias was added open git bash and enter the `alias` command
```sh
alias
```

![image](https://github.com/zackAJ/allias/assets/101515566/431dcfeb-eb56-4ab4-8e66-703d4b37386e)

5- test the alias by adding a repo name (my repo's name is alias)
```sh
clone alias
```

![image](https://github.com/zackAJ/alias/assets/101515566/f80abafa-a3db-499f-b065-d338a995a84e)

and that's it ! more copy-paste ready aliases are gonna be added soon.
