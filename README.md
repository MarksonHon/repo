# A bucket for Scoop providing Clash .NET 

Thanks to: <https://github.com/kidonng/sushi>

## Install Clash .NET

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

### 4. Install Clash .NET

```pwsh
scoop install clashdotnet
```

## Update Clash .NET

```pwsh
scoop update clashdotnet ### or use scoop update "*" to upgrade all scoop packages.
```

## Remove old version(s)

```pwsh 
scoop clean clashdotnet
```

## TIPS: 
1. Windows 7 users should install [Microsoft .NET Framework 4.8](https://support.microsoft.com/en-us/topic/microsoft-net-framework-4-8-offline-installer-for-windows-9d23f658-3b97-68ab-d013-aa3c3e7495e0) at first.
2. Windows 7 and Windows 8.1 users should install [`PowerShell`](https://aka.ms/powershell-release?tag=stable) at first and run `scoop` in **`PowerShell`** but NOT `Windows PowerShell` or you might meet error(s).
3. You should [set proxy to `git`](https://gist.github.com/evantoli/f8c23a37eb3558ab8765) to update buckets if you are in China, and you should add a terminal proxy to make sure that `scoop` works fine.

```pwsh
set http_proxy=http://proxyserver:1000 ### 1000 means your proxy server's port
set https_proxy=http://proxyserver:1000 
```
If you are using a proxy software such as Shadowsocks-Windows, proxyserver will be `localhost` or `127.0.0.1`.
