Dotfiles
========

Enjoy :)

Screenshots
-----------

![screenshot 1](/.md-resources/screenshot-1.jpg)

![screenshot 2](/.md-resources/screenshot-2.jpg)

![screenshot 3](/.md-resources/screenshot-3.jpg)

Requirements
------------

This is a loose list and will surely be updated as I install more things:

#### Software

+ mpd
+ ncmpcpp
+ python2.7
+ python3.6
+ fish
+ vim
+ polybar
+ wal
+ feh
+ i3-gaps
+ xorg-server
+ xorg-xinit
+ URxvt
+ urxvt-perls
+ Vundle

#### Fonts

+ Operator Mono
+ Wuncon Siji
+ Unifont
+ symbola
+ Material Icons
+ Noto Sans

Installation
------------

1\. Clone this repository to your home folder:

```shell
# Navigate to home directory
cd ~

# Clone repository
git clone https://github.com/jakehamilton/dotfiles.git

# Enter repository directory
cd dotfiles
```

2\. Install the packages you want using `stow`

```shell
# Any of these are valid package installs
stow fish
stow i3
stow vim
stow xdefaults
stow xinitrc
stow wallpapers
stow polybar
```

Customization
-------------

#### Wallpaper/Color Scheme
The wallpaper and color theme are set using `wal`. You will need to
modify the i3 configuration file to set the appropriate wallpaper:

```shell
# Enter the repository directory
cd dotfiles

# Open the configuration file in the editor
vim i3/.config/i3/config
```

#### Vim

`Vundle` is used to pull in plugins, so you'll need to have that
installed and then run the following to install all the plugins:

```shell
vim +PluginInstall
```

#### Fish

Fish is configured to update some globals in the file
`.config/fish/config.fish`. You'll likely want to remove those
depending on how you handle things on your system.

As well, I have a private set of scripts stored at `~/scripts`. These
aren't uploaded to the dotfiles repository because they contain private
information, so you'll either want to create that directory or remove
it from the fish configuration to avoid any errors.
