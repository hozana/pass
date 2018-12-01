# Passwords!

This is a repository containing the passwords of Hozana.
All of the passwords are encrypted.

## How to read a password?
You’ll need to have your GPG key setup and pass installed (see below).

```
pass show path/to/password
```

## How to get access to the password?
First you need to have `pass` installed.
- On macOS: `brew install pass`
- On Linux: `apt install pass`
- On Windows: Don’t know, don’t care

You will also need a GPG key. If you don’t already have one, generate it with `gpg --generate-key`.
Once you have the gpg key, get its id with `gpg --list-keys`. Then export the public key with
`gpg --export THE_KEY_ID >key.pub`. Finally, add your key in the `hozana/keyring` repository.

Then ask someone who already has access to the keys to give access to your key in the pass.
