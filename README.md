# Steps to commit signature verification using GPG 
---
Open Git Bash.
---
1. gpg --list-secret-keys --keyid-format=long  => Check for existing GPG keys
2. gpg --full-generate-key => Generate a new GPG key
3. gpg --armor --export <GPG key ID> => Show GPG key

---
4. Copy your GPG key, beginning with -----BEGIN PGP PUBLIC KEY BLOCK----- and ending with -----END PGP PUBLIC KEY BLOCK-----.
---

