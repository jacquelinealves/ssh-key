<div align="center">
    <h1>Generate SSH Key pair</h1>
</div>

- On terminal run:
```
ssh-keygen -t rsa -b 2048 -C "e-mail"
```

- Press enter. Output similar to the following is displayed:
```
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/user/.ssh/id_ed25519):
```

- Accept the suggested filename and directory, unless you are generating a deploy key or want to save in a specific directory where you store other keys.

You can also dedicate the SSH key pair to a specific host.

- Specify a passphrase:

```
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
```

A confirmation is displayed, including information about where your files are stored.

A public and private key are generated. Add the public SSH key to your git account and keep the private key secure.

- To add an SSH key to your git account:

```
cat ~/.ssh/id_rsa.pub
```

Copy and paste the entire code into the SSH Keys configuration repository to have access to the project.
