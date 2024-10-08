# WPS Office 应用程序配置（适用于 OEM 安装包）
本 Repo 中，包含着雨糖科技从各个 WPS Office 的定制安装包中，挖掘发现的定制参数。

# 如何使用
对于普通用户，我们推荐您直接下载我们的特别版程序。

[WPS Office 雨糖科技特别版](http://raincandy.tech/wpsoffice_umrse/ "WPS Office 雨糖科技特别版")

对于高级用户，可以将配置好的参数文件 (oem.ini) 放置到非定制版 WPS 安装包的同一路径，<br>
安装程序应该会自动调用此文件。

或者也可以将配置好的参数文件放置在程序的以下安装目录：
<安装目录>\office6\cfgs

请注意，较新版本加入了一些限制，请阅读下面的“重要提示”获取更多信息。

# 重要提示
从以下版本开始，程序加入了对配置文件的参数加密校验：

* 2019 专业版：11.8.2.12287
* 2023 专业版：12.8.2.17149
* 2023 个人版 / 商业版 32 位：12.1.0.17133
* 2023 个人版 64 位内测：12.1.0.17325

此外，从以下版本开始，oem.ini 在最后一行加入了整个配置文件的校验值：

* 2023 专业版：12.8.2.17838
* 2023 个人版 32 位：12.1.0.17133
* 2023 个人版 64 位内测：12.1.0.17325
* 2023 商业版 32 位：12.1.0.17150

安装程序会使用校验值对配置文件进行校验。如果失败，程序会直接忽略并删除安装包所在目录下的 oem.ini 文件。

根据向相关 Staff 证实，此校验一开始仅适用于个人版，并且随后已在金山办公内部推动其他版本（商业版、专业版）跟进。

这些更改直接导致了本配置文件中的明文参数将不会被程序所接受，目前暂无解决办法。

# 版权声明
*"WPS", the WPS logo, "WPS+" and "WPS 365" are trademarks or registered trademarks of Kingsoft Corporation. Copyright (C) Kingsoft Corporation. All Rights Reserved.*

*“WPS”、WPS 徽标、“WPS+” 和 “WPS 365”是北京金山办公软件股份有限公司的商标或注册商标。版权所有 (C) 北京金山办公软件股份有限公司、珠海金山办公软件有限公司、武汉金山办公软件有限公司、安徽金山办公软件有限公司、广州金山移动科技有限公司。保留所有权利。*
