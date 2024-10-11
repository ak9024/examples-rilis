# windows

> Please update your windows first.

Add `OpenSSH.Server~~~~0.0.1.0`

```shell
Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0
```

Start service `sshd`

```shell
Start-Service sshd
```

Enable `OpenSSH Server` to start automatic while booting.

```shell
Set-Service -Name sshd -StartupType 'Automatic'
```

```shell
rilis --cfg setup.toml
```

