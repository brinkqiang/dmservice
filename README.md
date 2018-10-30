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
To show service installation GUI:

        nssm install [<servicename>]

To install a service without confirmation:

        nssm install <servicename> <app> [<args> ...]

To show service editing GUI:

        nssm edit <servicename>

To retrieve or edit service parameters directly:

        nssm dump <servicename>

        nssm get <servicename> <parameter> [<subparameter>]

        nssm set <servicename> <parameter> [<subparameter>] <value>

        nssm reset <servicename> <parameter> [<subparameter>]

To show service removal GUI:

        nssm remove [<servicename>]

To remove a service without confirmation:

        nssm remove <servicename> confirm

To manage a service:

        nssm start <servicename>

        nssm stop <servicename>

        nssm restart <servicename>

        nssm status <servicename>

        nssm statuscode <servicename>

        nssm rotate <servicename>

        nssm processes <servicename>

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
