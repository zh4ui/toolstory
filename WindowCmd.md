# Windows Command Line

## tips

### install scoop

Set-ExecutionPolicy RemoteSigned -scope CurrentUser
 iex (new-object net.webclient).downloadstring('https://get.scoop.sh')

### set proxy for chocolatey

```
choco config set proxy http://localhost:8888
choco config set proxyUser bob
choco config set proxyPassword 123Sup#rSecur3
choco config set proxyBypassList "'http://localhost,http://this.location/'" #0.10.4 required
choco config set proxyBypassOnLocal true #0.10.4 required
```

source: [Explicit Proxy Settings](https://github.com/chocolatey/choco/wiki/Proxy-Settings-for-Chocolatey#explicit-proxy-settings)

### set proxy for scoop

```
scoop config proxy proxy.example.org:8080
```

Note that don't put `http://` in the proxy's address.

source: [Using Scoop behind a proxy](https://github.com/lukesampson/scoop/wiki/Using-Scoop-behind-a-proxy)


### user mode for choco

* https://superuser.com/questions/1095475/chocolatey-as-non-admin-user


## system utils

* where.exe helps you find the path of a command. [source](https://stackoverflow.com/questions/304319/is-there-an-equivalent-of-which-on-the-windows-command-line)
* `manage-bde` manage bitlocker device.

## external utils

* [win32-openssh](https://github.com/PowerShell/Win32-OpenSSH)