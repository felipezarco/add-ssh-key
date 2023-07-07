# Generate new SSH Key and add it to Github 

1. Generate ssh key *with your own email*.
```shell
ssh-keygen -t ed25519 -C "felipezarco@hotmail.com"
``` 

2. Press Enter 
```shell
(/c/Users/you/.ssh/id_ed25519): **[Press enter]**
```

3. Choose your password (not very hard since you will need it everytime) 

4. Check if below command outputs "Agent pid number"
```
eval "$(ssh-agent -s)"
``` 

5. Set the password to your private key (Optional on Windows)
```
ssh-add ~/.ssh/id_ed25519
``` 

6. Copy the generated SSH key
````
clip < ~/.ssh/id_ed25519.pub
````
Or
```
cat ~/.ssh/id_ed25519.pub
```

7. Go to Github profile menu > *Settings* > *SSH and GPG keys* and paste it!

8. Click the "Star" top-right button if this worked.

...
That's it! Do not forget to hit the ⭐ button if you are now using SSH instead of HTTPS!


