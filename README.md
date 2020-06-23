# pacman-packages

## Packages included with repository currently
* [`switch-ex-curl`](https://github.com/eXhumer/switch-ex-curl/) - v7.69.2 
* [`hacPack`](https://github.com/The-4n/hacPack) - v1.36-r2 
* [`hackBrewPack`](https://github.com/The-4n/hacBrewPack) - v3.05 

## How to add repository to pacman

### 1. Locally import and sign key required for repository
```
sudo pacman-key --recv 4E4A2F76EE374FEFA922BA58B79078F74FFDAD52
sudo pacman-key --lsign 4E4A2F76EE374FEFA922BA58B79078F74FFDAD52
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
