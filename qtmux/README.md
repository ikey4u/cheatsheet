# 安装依赖

```
MacOS:

    brew install reattach-to-user-namespace subversion git

Linux:

    sudo apt-get install xsel subversion git
```

# 安装


- 安装脚本

```
svn export https://www.github.com/ikey4u/q/trunk/qtmux/.tmux ~/.tmux
ln -s ~/.tmux/tmuxrc ~/.tmux.conf
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

- 进入 tmux 安装插件

```
    <prefix> + I
```

# Ubuntu 编译安装 tmux 2.7

```
sudo apt update

sudo apt install -y git

sudo apt install -y automake
sudo apt install -y build-essential
sudo apt install -y pkg-config
sudo apt install -y libevent-dev
sudo apt install -y libncurses5-dev

cd /tmp

wget https://github.com/tmux/tmux/releases/download/2.7/tmux-2.7.tar.gz
tar xf tmux-2.7.tar.gz && cd tmux-2.7
./configure && make
sudo make install

cd -
rm -fr /tmp/tmux-2.7
```
