# Generate new SSH Key and add it to Github 

1. Generate ssh key *with your own email*.
```shell
ssh-keygen -t ed25519 -C "felipezarco@hotmail.com"
``` 

2. Enter a file in which to save the key
```shell
(/c/Users/you/.ssh/id_ed25519): **[Press enter]**
```

3. Check if below command outputs "Agent pid number"
```
eval "$(ssh-agent -s)"
``` 

4. Set the password to your private key (Optional on Windows)
```
ssh-add ~/.ssh/id_ed25519
``` 

5. Copy the generated SSH key
````
clip < ~/.ssh/id_ed25519.pub
```` 

6. Go to Github profile menu > *Settings* > *SSH and GPG keys* and paste it!

7. Click the "Star" top-right button if this worked.
