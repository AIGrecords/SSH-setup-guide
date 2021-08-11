# GENERATING A NEW SSH KEY FOR YOUR GITHUB ACCOUNT

`$ ssh-keygen -t ed25519 -C "<your_email_address>"`

##On older Systems

`$ ssh-keygen -t rsa -b 4096 -C "<your_email_address>"`

## Output
> Generating public/private ed25519 key pair.

# NEXT STEP

> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Re-type passphrasse]


# ADDING YOUR SSH HEY TO THE SSH-AGENT

`$ eval "$(ssh-agent -s)"`

### Output

> Agent pid 59566

# THEN
`$ ssh-add ~/.ssh/id_ed25519`

## IF THE ABOVE METHOD DOESN'T WORK...

`$ ssh-agent /bin/sh`
`$ ssh-add $yourkey`
