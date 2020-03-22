# SSH

## Recipes

- Connect to host:

```bash
ssh -A username@server
```

> -A enables forwarding of the authentication agent connection. In other
> words you can connect to another ssh server from current ssh server

- Mount folder on host with `sshfs`:

```bash
sshfs username@server:/path-on-server/ ~/path-to-mount-point -o reconnect
```

- Copy over SSH (actually the best way is mounting with `sshfs`):

```bash
# from local to remote
scp file.txt username@server:/path-on-server/

# from remote to local
scp username@server:/path-on-server/file.txt  file.txt

# copy all files and folders recursively from local to remote
scp -r * username@server:/path-on-server/
```

- Add your SSH key to the ssh-agent:

```bash
ssh-add ~/path-to-key
```

## Links

- [ssh -A explained](https://superuser.com/questions/1376111/with-ssh-what-does-the-a-flag-do/1376118)
- [Copy files over SSH](https://www.simplified.guide/ssh/copy-file)
