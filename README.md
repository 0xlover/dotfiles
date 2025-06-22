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
It's an optimized, comfortable and more secure Chromium fork with [uBlock Origin](https://ublockorigin.com/)(which is pre-installed), [TTV LOL PRO](https://chromewebstore.google.com/detail/ttv-lol-pro/bpaoeijjlplfjbagceilcgbkcdjbomjd?hl=en) and [Unhook](https://chromewebstore.google.com/detail/unhook-remove-youtube-rec/khncfooichmfjbepaaaebmommgaepoid?hl=en) for a distraction free YouTube experience
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
* [Go](https://marketplace.visualstudio.com/items?itemName=golang.Go)
* [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
* [WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
* [Discord Rich Presence](https://marketplace.visualstudio.com/items?itemName=LeonardSSH.vscord)

### Spotify
You know what it is.
```ps
Spotify.Spotify
```
Using [Spicetify](https://spicetify.app/) which provides premium features such as a removing cringy ads and the ability to play songs in any order without paying for Spotify premiun plus cool customization!

### Discord
Again, you know what it is, required to use it and sad about it.
```ps
winget install Discord.Discord
```
Using [Moonlight](https://moonlight-mod.github.io/) which provides premium features such as high quality streams without paying for fucking Nitro and other things such as themes(which I don't actually use)!

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

### Windows Terminal
> [!NOTE]
> Should be pre-installed now
With the same font and colorscheme I use everywhere which are [Commit Mono](https://commitmono.com/) and [Aura](https://github.com/daltonmenezes/aura-theme)

### Additional
* Debloat Windows even more with [Windows 11 debloat](https://github.com/Raphire/Win11Debloat) or just run this instead of Atlas!
* Install all the often necessary(gaming) [redistributables](https://github.com/abbodi1406/vcredist)
* The Whatsapp Desktop [client](https://www.whatsapp.com/download)

### Discover
* [MPV](https://mpv.io/), a minimal and keybind heavy video player
* [OpenComic](https://github.com/ollm/OpenComic), the best books, comics and manga reader I have ever used
* [Vencord](https://vencord.dev/), a more popular Discord client mod

#### Fonts
* [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
* [GitHub Monaspace](https://monaspace.githubnext.com/)
* [Nerd Fonts](https://www.nerdfonts.com/font-downloads)

#### Colorschemes
* [Gruvbox Meterial](https://github.com/sainnhe/gruvbox-material)
* [Nord](https://github.com/shaunsingh/nord.nvim)
* [Dracula](https://github.com/Mofiqul/dracula.nvim)
* [Catppuccin](https://github.com/catppuccin/nvim)
* [Rose Pine](https://github.com/rose-pine/neovim)

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
xsel
cmatrix
sqlite 
go 
```
```
go install github.com/0xlover/auth/cmd/auth@latest
go install github.com/go-delve/delve/cmd/dlv@latest
go install github.com/pressly/goose/v3/cmd/goose@latest
```
