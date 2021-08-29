# Generate new SSH Key and add it to Github 

```ssh-keygen -t ed25519 -C "felipezarco@hotmail.com"``` [Use your own e-mail]

```Enter a file in which to save the key``` (/c/Users/you/.ssh/id_ed25519): [Press enter]

```eval "$(ssh-agent -s)"``` [You should see an Agent pid number]

```ssh-add ~/.ssh/id_ed25519``` [Set the password to your private key]

```clip < ~/.ssh/id_ed25519.pub``` [Copy the generated SSH key]

Go to Github profile menu > *Settings* >  *SSH and GPG keys* and paste it!
