### Visual Studio Code
`$ sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list`

or

`$ vim /etc/yum.repos.d/vscode.repo`

```
[code]
name=Visual Studio Code
baseurl=https://packages.microsoft.com/yumrepos/vscode
enabled=1
gpgcheck=1
gpgkey=https://packages.microsoft.com/keys/microsoft.asc
```

```
$ rpm-ostree refresh-md
$ rpm-ostree install code
$ reboot
```

### Sublime Text
`$ vim /etc/yum.repos.d/sublime-text.repo`

```
[sublime-text]
name=Sublime Text - x86_64 - Stable
baseurl=https://download.sublimetext.com/rpm/stable/x86_64
enabled=1
gpgcheck=1
gpgkey=https://download.sublimetext.com/sublimehq-rpm-pub.gpg
```
```
$ rpm-ostree refresh-md
$ rpm-ostree install sublime-text
$ reboot
```
