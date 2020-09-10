# pacman-packages

## Packages included with repository currently
* [`switch-ex-curl`](https://github.com/eXhumer/switch-ex-curl/) - v7.69.1-3 
* [`hacPack`](https://github.com/The-4n/hacPack) - v1.36-r2 
* [`hackBrewPack`](https://github.com/The-4n/hacBrewPack) - v3.05 

## How to add repository to pacman

### 1. Locally import and sign key required for repository
```
sudo pacman-key --recv C84A0AC14DDA558C2E48DF82068C85F7D5DC3FA5
sudo pacman-key --lsign C84A0AC14DDA558C2E48DF82068C85F7D5DC3FA5
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
