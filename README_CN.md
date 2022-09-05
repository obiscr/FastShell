# FastShell


<p> 

[简体中文](https://github.com/obiscr/FastShell/blob/main/README_CN.md)  |
[English](https://github.com/obiscr/FastShell/blob/main/README.md)

</p>


# 折扣 (Discount)

添加微信群或者加入Slack 享受折扣

+ Slack

  [点击加入Slack](https://join.slack.com/t/observercreator/shared_invite/zt-14g3dnzkx-FGJM_WgY~vj0bJINTHQSAA)

+ 加入微信群

  <img width=200 src="https://user-images.githubusercontent.com/28687074/188489998-9fee38f5-5183-4e4a-aa7f-c5d31074dcc6.png" alt="二维码">


## 介绍

Fast Shell 支持管理自定义的脚本，可以快速执行shell指令。支持的指令，取决于当前IDE所使用的Shell环境。Fast Shell 具有相当高的自由度。所有的指令完全由用户自己定义。

通过一个简短的 `command` 替换 `一个很长串的command`。并且集成到了 IDE 的 `Run Anything`，因此您可以很方便通过 `Double Ctrl` 来打开。

Fast Shell的目标是让您摆脱 `.bashrc` 或者 `.zshrc` 中的 **alias**。

如果您已经在 `.bashrc` 或者 `.zshrc` 定义了一些常用的指令，这完全没关系。您依然可以把他添加到FastShell来执行。

### 支持的版本

Fast Shell 将会支持 JetBrains 全平台 `2020.1` ~ `2021.3`，`2022` 版本发布以后，也会尽快支持。

![git-repo](https://user-images.githubusercontent.com/28687074/160279796-574b4bd9-170a-472d-9a4e-fa897866b051.png)


![linux-show](https://user-images.githubusercontent.com/28687074/160279800-9b388cdc-a687-488c-a1eb-17785f750272.gif)

如果指令的内容很多，您也可以将其写成脚本，然后通过 Fast Shell 调用脚本来执行它。

![exec-shell](https://user-images.githubusercontent.com/28687074/160279810-2371b3cd-57f9-487c-888c-27dd49e1fec0.gif)


## 使用

双击 `Ctrl`，输入 `fs`，会列出已经设置好的所有 Fast Shell 指令，双击执行或者选中后按下回车键即可执行。

您还可以添加一个自定义指令。点击 **Run Anything** 工具栏右上角的 ![](https://intellij-icons.jetbrains.design/icons/AllIcons/general/settings.svg) 即可打开打开设置来管理您的指令。

您也可以通过 `Settings/Preferences` > `Tools` > `Fast Shell` 来打开设置。

![add-command](https://user-images.githubusercontent.com/28687074/160279806-2120b040-72f3-4319-8c5c-055cb05fb305.gif)

## 在Windows平台运行

**Linux** 和 **Mac** 的大部分Shell指令都相同。因此可以基本上可以通用。但是在 **Windows** 上情况有些不同。Windows 有他自己独立的指令。

例如：

|  Windows PowerShell  | Linux/macOS  |
|  ----  | ----  |
| ipconfig  | ifconfig |
| Get-Content `filename` -Wait  | tailf / tail -F `filename` |

因此设置指令的时候需要确保当前的Shell环境支持所设置的指令。

![win-exec](https://user-images.githubusercontent.com/28687074/160281920-fb654a8d-f4fe-49ba-b552-7f00f0c292be.gif)

## 附录

### 设置当前Shell环境

`Settings/Preferences` > `Tools` > `Terminal` > `Shell Path`

![bash-env](https://user-images.githubusercontent.com/28687074/160279815-5fa10f79-f6bb-42a7-86e1-22417765dea4.png)
