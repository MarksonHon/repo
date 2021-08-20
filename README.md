Moved to

<https://gitlab.com/MarksonHo/sinnia>

NO UPDATE ANYMORE HERE.

# A bucket for Scoop providing Clash .NET 

[中文版本](https://github.com/MarksonHon/repo/blob/main/README-CN.md)

Thanks to: <https://github.com/kidonng/sushi>

## Install Scoop & add buckets

### 1. Install Scoop

Just follow <https://scoop.sh/>

Gitee's installer mirror: <https://gitee.com/RubyKids/scoop-cn>

After installing Scoop, you should install git a first:

```pwsh
scoop install git
```

### 2. Add sushi bucket

Just follow <https://github.com/kidonng/sushi>

### 3. Add this bucket

```pwsh
scoop bucket add clashdotnet https://github.com/MarksonHon/repo/
```
## Install apps

### Clash .NET

```pwsh
scoop install clashdotnet
```

### Clash.Mini

```pwsh
scoop install clashmini
```

## Update apps

```pwsh
scoop update; scoop update "*"
```

## Remove old version(s)

```pwsh 
scoop cleanup "*"
```

## TIPS: 
1. Windows 7 users should install [Microsoft .NET Framework 4.8](https://support.microsoft.com/en-us/topic/microsoft-net-framework-4-8-offline-installer-for-windows-9d23f658-3b97-68ab-d013-aa3c3e7495e0) at first.
2. You should install [`PowerShell`](https://aka.ms/powershell-release?tag=stable) at first and run `scoop` in **`PowerShell`** but NOT `Windows PowerShell` or you might meet error(s).
3. You should [set proxy to `git`](https://gist.github.com/evantoli/f8c23a37eb3558ab8765) to update buckets if you are in China, and you should add a terminal proxy to make sure that `scoop` works fine.

```pwsh
$env:HTTP_PROXY="http://127.0.0.1:11223" ### 11223 means your proxy server's port
$env:HTTPS_PROXY="http://127.0.0.1:11223"
$env:ALL_PROXY="socks5://127.0.0.1:11223"
```
If you are using a proxy software such as Shadowsocks-Windows, proxyserver will be `localhost` or `127.0.0.1`.
