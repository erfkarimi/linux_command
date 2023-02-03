### ZSH installation
```bash
sudo dnf install zsh
```
### ohmyzsh installation
```bash
sudo dnf install wget curl git

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

OR

sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"

chsh -s $(which zsh)
```