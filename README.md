# prflab

This is the handout directory for prflab - a lab that teaches you how to exploit hardware and systems-software to write high-performance software. Make sure to read the above-URL'ed PDF before you proceed.

This README details how you should handle this assignment:

1. [Setting up clab](#setting-up-clab)
2. [Doing the assignment](#doing-the-assignment)
3. [Submitting your work](#submitting-your-work)


## Setting up prflab
You must fork this repository to your own user account and work on the
assignment from that fork. When you are done, you should create a pull request
against the original repository.


### Fork repository
The following images illustrate how to fork the course repository.

First press the Fork-button on the lab repository:
![Fork](https://github.itu.dk/pages/OSC/23-Website/images/Fork.png)


You may have to select the organisation or owner of the fork.<br>
Select your ITU username:
![ChooseUser](https://github.itu.dk/pages/OSC/23-Website/images/ChooseUser.png)


When forked, we need to get the repository’s URL to clone from.<br>
If you press `Use HTTPS` at the top of the popup box (see image below), you
will authenticate against github with ITU username and password instead of
ssh keys (see [this link](https://devconnected.com/how-to-setup-ssh-keys-on-github/)
for information on how to use SSH keys to interact with GitHub).
![GetCloneUrl](https://github.itu.dk/pages/OSC/23-Website/images/GetCloneUrl.png)


### Setup your working copy of the repo
Switch to a terminal (logged in to the course server, for instance) and do the
following:
```
# Download git repository (replace nhed with your own user name)
git clone git@github.itu.dk:nhed/prflab24.git prflab

# Change into cloned directory
cd prflab

# Checkout your branch (replace nhed with your own user name)
git checkout -b nhed

# Make initial push to remote to set upstream clone URL (replace nhed with your own user name)
git push -u origin nhed
```

## Doing the assignment
You should now have access to the course files on your user account and have set
up a tracking branch corresponding to your username on your own fork of the
repository.<br>
Add your changes to a commit by using 

```
git add kernels.c
```

Commit your changes by writing 

```
git commit -m "<some commit message>"
```

and push them to your branch using 

```
git push -u origin initials
``` 

After this, you should be tracking your branch, meaning that you can simply write `git push` to upload your changes.

When you are satisfied with your changes/results you should create a pull request using github.itu.dk's web interface and name it like `initials / attempt #` or something along those lines.