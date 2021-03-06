移动到：
<https://gitlab.com/MarksonHo/sinnia>

此处不再更新。

# 一个 Scoop 仓库

特别鸣谢 <https://github.com/kidonng/sushi>

## 安装 Scoop、添加仓库

### 1. 安装 Scoop

只要按照 <https://scoop.sh/> 的说明来完成安装即可。

Gitee 的安装程序镜像：<https://gitee.com/RubyKids/scoop-cn>

安装完 Scoop 后，你应该先安装 git：

```pwsh
scoop install git
```

### 2. 添加 sushi 仓库

只需遵循 <https://github.com/kidonng/sushi>

### 3. 添加本仓库

```pwsh
scoop bucket add clashdotnet https://github.com/MarksonHon/repo/
```

## 安装软件

### Clash .NET

```pwsh
scoop install clashdotnet
```
### Clash.Mini

```pwsh
scoop install clashmini
```

## 升级软件

```pwsh
scoop update; scoop update "*"
```

## 移除旧版本

```pwsh 
scoop cleanup "*"
```

## 提示: 

1. Windows 7 用户应该先安装[Microsoft .NET Framework 4.8](https://support.microsoft.com/en-us/topic/microsoft-net-framework-4-8-offline-installer-for-windows-9d23f658-3b97-68ab-d013-aa3c3e7495e0)。
2. 你应首先安装[`PowerShell`](https://aka.ms/powershell-release?tag=stable)，并在 **`PowerShell`** 中运行`scoop`，而不是`Windows PowerShell`，否则你可能会遇到错误。
3. 如果你在中国，你应该 [给`git`配置代理](https://gist.github.com/evantoli/f8c23a37eb3558ab8765) 以便更新仓库，同时你应该添加一个终端代理来确保 `scoop` 工作正常。

    ```pwsh
    $env:HTTP_PROXY="http://127.0.0.1:11223"
    $env:HTTPS_PROXY="http://127.0.0.1:11223"
    $env:ALL_PROXY="socks5://127.0.0.1:11223"
    ```
    如果你使用代理软件，如 Shadowsocks-Windows，proxyserver将是`localhost`或`127.0.0.1`。
