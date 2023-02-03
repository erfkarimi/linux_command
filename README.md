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

### snap installation
```bash 
sudo dnf install snapd

sudo ln -s /var/lib/snapd/snap /snap
```

### VLC installation
```bash
sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm 

sudo dnf install vlc
```

### Nvidia graphic card driver
```bash
sudo dnf upgrade --refresh -y

sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm

sudo dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

sudo dnf update --refresh

sudo dnf install akmod-nvidia -y

sudo dnf install xorg-x11-drv-nvidia-cuda
```

### Docker installation
```bash
sudo dnf -y install dnf-plugins-core

sudo dnf config-manager \
    --add-repo \
    https://download.docker.com/linux/fedora/docker-ce.repo

sudo dnf install docker-ce docker-ce-cli containerd.io docker-compose-plugin

sudo systemctl start docker

sudo docker run hello-world
```


