## System Preferences
    General
        Appearance -> "Auto"
    Dock & Menu Bar
        Dock & Menu Bar
            Automatically hide and show the Dock -> [x]
        Clock
            Use a 24-hour clock -> [x]
            Display the time with seconds -> [x]
    Trackpad
        Point & Click
            Tap to click -> [x]
            Click -> "Firm"
        More Gestures
            Swipe between full-screen apps -> "Swipe left or right with four fingers"
            Swipe between pages -> "Swipe with three fingers"
    Keyboard
        Keyboard
            Key Repeat -> "Fast"
        Input Sources -> Add Dvorak
    Security & Privacy
        Location Services
            Enable Location Services -> [x]
    Date & Time
        Time Zone
            Set time zone automatically using current location -> [x]

## Manual Installs
- nix-env
- logitech options
- Parallels
- CleanMyMacX
- Adobe Photoshop
- Infuse Video Player

## Brew
Manually install [brew](https://brew.sh/)

`brew bundle Brewfile`

## Dotfiles
```
git clone git@github.com:upaymeifixit/dotfiles.git
cd dotfiles
./link
```
# [Fisher](https://github.com/jorgebucaran/fisher)
Install: `curl -sL https://raw.githubusercontent.com/jorgebucaran/fisher/main/functions/fisher.fish | source && fisher install jorgebucaran/fisher`

Run: `fisher install`


# Other
## Sync Signal
Copy files in the following directories:
- `~/Library/Caches/org.whispersystems.signal-desktop`
- `~/Library/Saved\ Application\ State//org.whispersystems.signal-desktop.savedState`
- `~/Library/Caches/org.whispersystems.signal-desktop.ShipIt`
- `~Library/Application\ Support/Signal`

Deauthorize the device via app and re-authorize both devices


## Set up SSH keys
### Example
`ssh-keygen -t ed25519 -f ~/.ssh/paciolan-bitbucket_ed25519; and cat ~/.ssh/paciolan-bitbucket_ed25519.pub | pbcopy`

Paste contents into other machine's ~/.ssh/authorized_keys file

Create entry in ~/.ssh/config similar to this:
```
Host Joshs-Hackintosh
	HostName 10.0.1.1
	User josh
    Port 22
	IdentityFile ~/.ssh/joshs-hackintosh_ed25519
	IdentitiesOnly yes
```


STILL NEED TO:
