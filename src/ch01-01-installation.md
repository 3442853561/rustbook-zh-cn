## 安装

使用 Rust 的第一步就是安装它。
在运行本章中的命令时您需要连接网络。
因为我们将从互联网上下载 Rust。

我们将使用终端的形式展示一些命令，这些命令都是以 `$` 开头的。
您不需要输入字符 `$` ；它们只是为了表示命令行的开端。
您会在网上看到许多遵循此约定的教程和示例：
`$` 作为系统普通用户可以运行的命令，
`#` 作为系统管理员用户可以运行的命令。
不以 `$` 开头的行通常是上一个命令的输出。

### 在 Linux 或 Mac 上安装

如果您使用的是 Linux 或 Mac，
您只需要打开一个终端并输入：

```text
$ curl https://sh.rustup.rs -sSf | sh
```

它将会下载一个脚本并开始安装，
系统可能会提示您输入密码。
如果顺利的话，您将会看到：

```text
Rust is installed now. Great!
```

当然，如果您不同意使用 `curl | sh` 模式，
您也可以以您喜欢的方式下载、检查并运行脚本。

### 在 Windows 上安装

在 Windows 上，请您打开 [https://rustup.rs](https://rustup.rs/) 并按照说明下载 rustup-init.exe。
运行它并按照它给您的其他提示进行操作。

本书中的其他 Windows 特定命令，
假设您会使用 `cmd` 作为 shell。如果您使用的是不同的 shell ，
您可以运行与 Linux 和 Mac 用户相同的命令。
如果以上两种方式都不能正常运行，
请参阅您正在使用的 shell 的文档。

### 自定义安装

如果您因为某些原因不愿意使用 rustup.rs 。
请在 [Rust 安装页面](https://www.rust-lang.org/install.html) 中了解其他选项。

> Rust 安装页面的中文本土化页面是 https://www.rust-lang.org/zh-CN/install.html 

### 卸载

卸载 Rust 和安装它一样简单。
您只需要打开终端并运行卸载脚本：

```text
$ rustup self uninstall
```

### 故障排除

如果您已经安装了 Rust，
您可以打开一个 shell 并输入：

```text
$ rustc --version
```

您应该能看到类似以下格式的在您安装时的最新稳定版本的版本号、
提交哈希(commit hash)及提交日期：

```text
rustc x.y.z (abcabcabc yyyy-mm-dd)
```

如果你看到了这条信息，
恭喜您 Rust 已经成功安装了！

如果您没有安装成功，并且您使用的是 Windows 操作系统，
请检查 Rust 是否在您的 `%PATH%` 环境变量。

如果它仍然不能运行，您可以在这些地方得到帮助。
其中最简单的则是 [irc.mozilla.org 上的 #rust IRC 频道][irc]，
您可以通过 [Mibbit][mibbit]访问它。点击此地址，
您可以和其他 Rustaceans（Rust开发者的昵称）聊天，
我们可以帮助您。还有一些包括[用户论坛][users]和 [Stack Overflow][stackoverflow] 在内的绝佳资源。

> 您可以在微博上获得中文帮助。我们的微博账号是[@Rust语言][weibo]。

[irc]: irc://irc.mozilla.org/#rust
[mibbit]: http://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust
[users]: https://users.rust-lang.org/
[stackoverflow]: http://stackoverflow.com/questions/tagged/rust
[weibo]: http://weibo.com/u/5616913483

### 本地文档

安装程序还包括了一份本地文档的副本，
所以您可以离线阅读它。
运行 `rustup doc` 在您的浏览器中打开本地文档。

每当有一个您不确定的由标准库提供的类型或函数时，
您都可以在 API 文档找到它。
