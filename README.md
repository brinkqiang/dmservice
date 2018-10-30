# dmservice

Copyright (c) 2013-2018 brinkqiang (brink.qiang@gmail.com)

[dmservice GitHub](https://github.com/brinkqiang/dmservice)

## Build status
| [Linux][lin-link] | [MacOSX][osx-link] | [Windows][win-link] |
| :---------------: | :----------------: | :-----------------: |
| ![lin-badge]      | ![osx-badge]       | ![win-badge]        |

[lin-badge]: https://travis-ci.org/brinkqiang/dmservice.svg?branch=master "Travis build status"
[lin-link]:  https://travis-ci.org/brinkqiang/dmservice "Travis build status"
[osx-badge]: https://travis-ci.org/brinkqiang/dmservice.svg?branch=master "Travis build status"
[osx-link]:  https://travis-ci.org/brinkqiang/dmservice "Travis build status"
[win-badge]: https://ci.appveyor.com/api/projects/status/github/brinkqiang/dmservice?branch=master&svg=true "AppVeyor build status"
[win-link]:  https://ci.appveyor.com/project/brinkqiang/dmservice "AppVeyor build status"

## Intro
dmservice

windows 使用nssm实现
```
nssm install <servicename>
nssm install <servicename> <program> [<arguments>]
nssm start <servicename>
nssm stop <servicename>
nssm restart <servicename>
nssm edit <servicename>
nssm remove <servicename>
nssm remove <servicename> confirm

如下是一个安装Jenkins服务的示例：
nssm install Jenkins %PROGRAMFILES%\Java\jre7\bin\java.exe
nssm set Jenkins AppParameters -jar slave.jar -jnlpUrl https://jenkins/computer/%COMPUTERNAME%/slave-agent.jnlp -secret redacted
nssm set Jenkins AppDirectory C:\Jenkins
nssm set Jenkins AppStdout C:\Jenkins\jenkins.log
nssm set Jenkins AppStderr C:\Jenkins\jenkins.log
nssm set Jenkins AppStopMethodSkip 6
nssm set Jenkins AppStopMethodConsole 1000
nssm set Jenkins AppThrottle 5000
nssm start Jenkins

```

linux 待定
```
```
## Contacts
[![Join the chat](https://badges.gitter.im/brinkqiang/dmservice/Lobby.svg)](https://gitter.im/brinkqiang/dmservice)

## Thanks
