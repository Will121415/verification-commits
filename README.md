# Steps to commit signature verification using GPG 
---
Open Git Bash.
---
1. gpg --list-secret-keys --keyid-format=long  => Check for existing GPG keys
2. gpg --full-generate-key => Generate a new GPG key
3. gpg --armor --export <GPG key ID> => Show GPG key
4. Copy your GPG key, beginning with -----BEGIN PGP PUBLIC KEY BLOCK----- and ending with -----END PGP PUBLIC KEY BLOCK-----.
5. Add the GPG key to your GitHub account.
6. git config --global commit.gpgsign true  => To sign all commits by default in any local repository on your computer, run
7. git config --global user.signingkey <GPG key ID> =>  Telling Git about your signing key
---
When committing changes in your local branch, add the -S flag to the git commit command:
$ git commit -S -m "your commit message"
--- 


