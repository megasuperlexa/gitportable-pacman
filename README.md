# gitportable-pacman

Script to install pacman in git for Windows portable

Run `sh install-pacman-git-bash.sh` from a git-bash session.

Install zshell `Pacman -S zsh`

# OR
(didn't try yet)
Just use chocolatey:
```
choco install msys2-installer
pacman -Sy zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

# oh-my-zsh
Clone oh-my-zsh
```
git clone https://github.com/ohmyzsh/ohmyzsh.git
cp -r ~/ohmyzsh/. ~/.oh-my-zsh
```

Add some plugins

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Clone powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
```
Add everything in [`.zshrc`](.zshrc_sample)

Create `~\.bashrc`:
```
export SHELL=/bin/zsh
exec /bin/zsh
```


