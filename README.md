# azl-livecd
A LiveCD for AzureLinux

## Description

If you want to try the Azurelinux 3.0 distribution from Microsoft, but don't want to install an ISO, run a VM or use WSL, here's a LiveCD that you can use.

## How to use

On a hypervisor (KVM, HyperV, etc) boot the ISO.

```
username: azl
password: azl
```

## FAQ

- Does it have ssh server enabled by default?

No, since it has a default password, openssh server is not enabled. For that, run:

```
sudo tdnf install openssh
sudo systemctl enable sshd
```

