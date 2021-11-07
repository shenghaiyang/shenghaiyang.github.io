# Homebrew

## 使用`ustc`源安装

```shell

# 第一步，创建文件夹
sudo mkdir /usr/local/Homebrew

# 第二步：git克隆
sudo git clone https://mirrors.ustc.edu.cn/brew.git /usr/local/Homebrew

# 第三步：创建一个快捷方式到/usr/local/bin目录
sudo ln -s /usr/local/Homebrew/bin/brew /usr/local/bin/brew

# 第四步：创建core文件夹 并 再次git克隆
sudo mkdir -p /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core
sudo git clone https://mirrors.ustc.edu.cn/homebrew-core.git /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core

# 第五步：获取权限 并 运行更新
sudo chown -R $(whoami) /usr/local/Homebrew
brew update

# 最后设置：设置环境变量
export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles

```