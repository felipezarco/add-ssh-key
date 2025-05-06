# How to Generate SSH Key and Add it to Github (step by step)

1. Generate ssh key *with your own email*.
```shell
ssh-keygen -t ed25519 -C "felipezarco@hotmail.com"
``` 

2. Press Enter when
(/c/Users/you/.ssh/id_ed25519): **[Press enter]**

3. Leave it empty for no password OR choose your password (not very hard since you will need it everytime) 

4. Check if command below correctly outputs "Agent pid" with some number

```
eval "$(ssh-agent -s)"
``` 

5. Set the password to your private key (Optional on Windows)

```
ssh-add ~/.ssh/id_ed25519
``` 

6. Copy the generated SSH key:
```
cat ~/.ssh/id_ed25519.pub
```

7. Go to Github profile menu > *Settings* > *SSH and GPG keys* (or just [click here](https://github.com/settings/ssh/new)), give it a name to identify the computer and paste it!

8. Do not forget to hit the ⭐ button if this worked 😉 !

That's it!
...


Above SSH configuration is a solution to the following meesage (i.e.lack of repository access).

```
The authenticity of host 'github.com (20.201.28.151)' can't be established.
ED25519 key fingerprint is XXXXXXXXX.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

