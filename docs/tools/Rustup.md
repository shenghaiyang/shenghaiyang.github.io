# Rustup

## 配置Crates源

在`$HOME/.cargo/config`中添加如下内容：

```toml
[source.crates-io]
replace-with = 'ustc'

[source.ustc]
registry = "git://mirrors.ustc.edu.cn/crates.io-index"
```

如果所处的环境中不允许使用 git 协议，可以把上述地址改为：

```toml
registry = "https://mirrors.ustc.edu.cn/crates.io-index"
```

## Rust Toolchain 反向代理

使用 rustup 前，先设置环境变量 RUSTUP_DIST_SERVER （用于更新 toolchain）：

```shell
export RUSTUP_DIST_SERVER=https://mirrors.ustc.edu.cn/rust-static
```

以及 RUSTUP_UPDATE_ROOT （用于更新 rustup）：

```shell
export RUSTUP_UPDATE_ROOT=https://mirrors.ustc.edu.cn/rust-static/rustup
```
## Rustup 安装

第一次安装`rustup`的时候，如果按照官网教程`https://sh.rustup.rs`链接无法下载，可以通过[jsDelivrCDN](https://cdn.jsdelivr.net/gh/rust-lang-nursery/rustup.rs/rustup-init.sh)下载`rustup-init.sh`，然后把脚本中的`RUSTUP_UPDATE_ROOT`变量改为`https://mirrors.ustc.edu.cn/rust-static/rustup。`