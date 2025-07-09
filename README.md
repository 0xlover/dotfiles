# Dotfiles
> Pragmatic and comfy setup on the latest Windows with Arch Linux inside WSL!

# Steps to reproduce
1. Install the latest Windows version
2. Complete Windows Updates
3. Run the [Atlas](https://atlasos.net/) playbook with the [AME installer](https://ameliorated.io/)
5. Enable WSL2 and install [Arch Linux](https://archlinux.org/)(wsl.exe --install -d archlinux")
5. Get whatever applications you need and install my/your dotfiles

> [!WARNING]
> Atlas will provide a leaner and more performant system by heavily modifying your Windows installation, be sure that's what you want!

## Applications
### Thorium
It's an optimized, comfortable and more secure Chromium fork with [uBlock Origin](https://ublockorigin.com/)(which is pre-installed), [TTV LOL PRO](https://chromewebstore.google.com/detail/ttv-lol-pro/bpaoeijjlplfjbagceilcgbkcdjbomjd?hl=en), [Unhook](https://chromewebstore.google.com/detail/unhook-remove-youtube-rec/khncfooichmfjbepaaaebmommgaepoid?hl=en) for a distraction free YouTube experience and [Violentmonkey](https://violentmonkey.github.io/) with [AdGuard PopupBlocker](https://github.com/AdguardTeam/PopupBlocker)
```ps
winget install Alex313031.Thorium
```

### HTTPie
The best HTTP client I have used that doesn't get in the fucking way
```ps
winget install HTTPie.HTTPie
```

### Visual Studio Code
My graphical editor of choice, in a shell(maybe over SSH) I use Neovim or whatever Vi variant is available!
```ps
winget install Microsoft.VisualStudioCode --override "/verysilent /suppressmsgboxes /mergetasks='!runcode,addcontextmenufiles,addcontextmenufolders,associatewithfiles,addtopath'"
```
These crazy looking flags just adds it to the context menu, append it to the $env:Path and associate various file types which you probably want!

#### Extensions
* [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
* [WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
* [Go](https://marketplace.visualstudio.com/items?itemName=golang.Go)
* [Bun](https://marketplace.visualstudio.com/items?itemName=oven.bun-vscode)
* [Tinymist](https://marketplace.visualstudio.com/items?itemName=myriad-dreamin.tinymist)
* [Biome](https://marketplace.visualstudio.com/items?itemName=biomejs.biome)

### Spotify
You know what it is.
```ps
Spotify.Spotify
```
Using [Spicetify](https://spicetify.app/) which provides premium features such as a removing cringy ads and the ability to play songs in any order without paying for Spotify premiun plus cool customization!

### More
* Anki(for my japanese studies)
```ps
winget install Anki.Anki
```
* Bitwarden(for my password needs)
```ps
winget install Bitwarden.Bitwarden
```
* OBS(needs no presentation)
```ps
winget install OBSProject.OBSStudio
```
* CupCut(for my editing needs)
```ps
winget install ByteDance.CapCut
```
* VLC(preferred video player)
```ps
winget install VideoLan.VLC 
```
* Google Drive(it's just what I use for backups)
```ps
winget install Google.GoogleDrive
```
* qBittorrent(preferred torrent client)
```ps
winget install qBittorrent.qBittorrent
```
* OpenComic(the best books, comics and manga reader I have ever used)
```ps
Get it from https://github.com/ollm/OpenComic/releases
```

### Windows Terminal
> [!NOTE]
> Should be pre-installed now
With the same font and colorscheme I use everywhere which are [Commit Mono](https://commitmono.com/) and [GitHub Dark](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme)

### Additional
* Debloat Windows even more with [Windows 11 debloat](https://github.com/Raphire/Win11Debloat) or just run this instead of Atlas!
* Install all the often necessary(gaming) [redistributables](https://github.com/abbodi1406/vcredist)
* The Whatsapp Desktop [client](https://www.whatsapp.com/download)

### Inside Arch Linux WSL2
```
base-devel 
binutils 
file 
which 
tree
sudo
man-db 
bash-completion
curl 
wget
aria2 
openssh
openssl
aws-cli
azure-cli 
terraform 
bc 
fd 
ripgrep
git 
git-lfs 
go
neovim 
neovide
xsel
sqlite 
ollama
go 
```
```
go install github.com/0xlover/auth/cmd/auth@latest
go install github.com/0xlover/vuln/cmd/vuln@latest
go install github.com/go-delve/delve/cmd/dlv@latest
go install github.com/pressly/goose/v3/cmd/goose@latest
go install github.com/ffuf/ffuf/v2@latest
go install github.com/gohugoio/hugo@latest
```
