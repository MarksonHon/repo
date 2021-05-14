# A bucket for Scoop providing Clash .NET 

Thanks to: <https://github.com/kidonng/sushi>

## 1. Install Scoop

Just follow <https://scoop.sh/>

Or you can use this command to get better speed in China (thanks to [kidonng](https://github.com/kidonng)):

```pwsh
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
iwr -useb 'https://raw.fastgit.org/kidonng/scoop-install/fastgit/install.ps1' | iex
```

After installing Scoop, you should install git a first:

```pwsh
scoop install 

## 2. Add sushi bucket

Just follow <https://github.com/kidonng/sushi>

## 3. Add this bucket

```pwsh
scoop bucket add clashdotnet https://github.com/MarksonHon/repo/
```

## 4. Install Clash .NET

```pwsh
scoop install clashdotnet
```
