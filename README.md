# Generate new SSH Key and add it to Github 

1. ```ssh-keygen -t ed25519 -C "felipezarco@hotmail.com"``` **[Use your own e-mail]**

2. ```Enter a file in which to save the key``` (/c/Users/you/.ssh/id_ed25519): **[Press enter]**

3. ```eval "$(ssh-agent -s)"``` **[You should see an Agent pid number]**

4. ```ssh-add ~/.ssh/id_ed25519``` **[Set the password to your private key]** (Optional on Windows)

5. ```clip < ~/.ssh/id_ed25519.pub``` **[Copy the generated SSH key]**

**Go to Github profile** menu > *Settings* >  *SSH and GPG keys* and paste it!
