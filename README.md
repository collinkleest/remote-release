# remote-release

Action for running a remote release wrapper around [appleboy/ssh-action](https://github.com/appleboy/ssh-action)

### Usage

```yaml
- uses: collinkleest/remote-release@v1
  with:
    # Hostname or IP address of remote server (i.e. 192.168.1.1 or example.com)
    # required
    host: ""
    # Port number of ssh server running on remote server
    # optional (defaults to 22)
    port: 22
    # Username to log in under for ssh on the remote server
    # required
    username: ""
    # Password to log into the ssh server on the remote server
    # required
    password: ""
    # Target directory where you want the deployed code to go
    # optional (defaults to ~/github)
    target-directory: ""
    # Release command to run in the context of the repo
    # optional (defaults to docker compose down && docker compose up -d)
    command: ""
    # Amount of time alloted until the command times out
    # optional (defaults to 15m)
    command_timeout: ""
```

### For releasing (internal use)

See [RELEASE.md](./RELEASE.md)
