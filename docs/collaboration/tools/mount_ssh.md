
# how to work with a remote filesystem over ssh

## OSX

### opensource way on OSX

- install: https://osxfuse.github.io/
- ```brew install sshfs```

how to mount

```bash
mkdir -p ~/mount/threefoldfoundation
sshfs root@165.22.206.215:/sandbox/code/github/threefoldfoundation/ ~/mount/threefoldfoundation

```

### free useful software

- https://cyberduck.io/download/ can be used to synchronize the relevant directories to edit


## Windows

- https://www.digitalocean.com/community/tutorials/how-to-use-sshfs-to-mount-remote-file-systems-over-ssh

