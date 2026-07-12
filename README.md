# WPS Office 应用程序配置（适用于 OEM 安装包）
本 Repo 中，包含着雨糖科技从各个 WPS Office 的定制安装包中，挖掘发现的定制参数。

# 如何使用
对于普通用户，我们推荐您直接下载我们的特别版程序。

[WPS Office 雨糖科技特别版](http://raincandy.tech/wpsoffice_umrse/ "WPS Office 雨糖科技特别版")

对于高级用户，可以将配置好的参数文件 (oem.ini) 放置到非定制版 WPS 安装包的同一路径，<br>
安装程序应该会自动调用此文件。

# 目录对应程序版本
* Conf_Internal_10：2016 内测版
* Conf_Internal_11：2019 内测版
* Conf_Internal_12：2023 内测版
* Conf_Internal_12_Sherii：2023 内测版（新 12.1.0 分支专业版）
* Conf_Internal_Personal：2023 内测版（个人版 / 商业版老版，已废弃）
* Conf_Production_10：2016 外发版
* Conf_Production_11：2019 外发版
* Conf_Production_12：2023 外发版
* Conf_Production_12_Sherii：2023 外发版（新 12.1.0 分支专业版）
* Conf_Production_PDF_11：金山 PDF 专业版 2019 外发版
* Conf_Production_PDF_12：WPS PDF 专业版 2023 外发版
* Conf_Production_PDF_12_Sherii：WPS PDF 专业版 2023 外发版（新 PDF & OFD 融合独立版）

内测版配置文件有详细参数说明，外发版没有。

# 如何获取非定制版安装包
在非定制版的 WPS 安装包的文件属性中，您可以看到其原始文件名以 "KPacket" 打头。

可以使用 7-Zip 打开定制版安装包，将 `$_11_` 文件夹中的 $EXEFILE 提取出来，删除 $ 符号并添加 .exe 后缀名即可。

# 关于参数加密编码

从以下程序版本开始，必须对参数进行加密编码：

* 2019 专业版：11.8.2.12287
* 2023 专业版：12.8.2.17149
* 2023 个人版 / 商业版 32 位：12.1.0.17133
* 2023 个人版 64 位内测：12.1.0.17325

这些更改直接导致了本配置文件中的明文参数将不会被程序所接受。这时候，您应该使用文件名标注有“cipher”的配置文件。

您也可以使用雪狐编写的 [WPSProfileCipher](https://github.com/NixaVulpi/WPSProfileCipher) 工具对参数进行加解密。

# 关于配置文件总校验

从以下版本开始，oem.ini 在最后一行加入了整个配置文件的校验值：

* 2019 专业版：11.8.2.12344
* 2023 专业版：12.8.2.17838
* 2023 个人版 32 位：12.1.0.17133
* 2023 个人版 64 位内测：12.1.0.17325
* 2023 商业版 32 位：12.1.0.17150

已知主程序和安装程序均会使用校验值对配置文件进行校验。

# 关于配置参数的格式更新
WPS Office 2023 从以下版本开始，金山办公对配置文件的参数格式进行了修改：

* 32 位：待补充（专业版已知从 12.1.0.23542 开始）
* 64 位：待补充（专业版已知从 12.1.0.23122 开始）

因此请注意，旧版本的配置文件在新版本中已经不再可用。

# 版权声明
*"WPS", the WPS logo, "WPS+" and "WPS 365" are trademarks or registered trademarks of Kingsoft Corporation. Copyright (C) Kingsoft Corporation. All Rights Reserved.*

*“WPS”、WPS 徽标、“WPS+” 和 “WPS 365”是北京金山办公软件股份有限公司的商标或注册商标。版权所有 (C) 北京金山办公软件股份有限公司、珠海金山办公软件有限公司、武汉金山办公软件有限公司、安徽金山办公软件有限公司、广州金山移动科技有限公司。保留所有权利。*
