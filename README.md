# pacman-packages

## Packages included with repository currently
* [`libnx-git`](https://github.com/switchbrew/libnx/) - master

## How to add repository to pacman

### 1. Locally import and sign key required for repository
```
sudo pacman-key --keyserver keyserver.ubuntu.com --recv-keys 13105126BA2E3B99C2923C9A3A1CA61549E890F3
sudo pacman-key --lsign 13105126BA2E3B99C2923C9A3A1CA61549E890F3
```

### 2. Add "server" information for repository locally
**NOTE: This needs to be added to `/etc/pacman.conf` file**
```
[ex-repo]
Server = https://github.com/eXhumer/pacman-packages/releases/latest/download/
```

### 3. Refresh and sync all repositories
```
sudo (dkp-)pacman --sync --refresh
```
