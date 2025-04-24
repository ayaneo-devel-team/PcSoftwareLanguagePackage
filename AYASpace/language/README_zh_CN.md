​	如果当前的 AYASpace 语言不包含您的国家，您也可以在 AYASpace 安装目录/language 文件夹中添加语言文件并修改配置文件 `config.json`，或者修改现有语言文件（请注意， AYASpace 升级可能会覆盖，因此您需要在升级前备份文件）。



`config.json` 可配置为在 AYASpace 设置/通用/语言 列表中显示

```json
[
    {
        "language": "zh_CN",
        "name": "简体中文",
        "filename": "zh_CN.json"
    },
    {
        "language": "zh_TW",
        "name": "繁體中文",
        "filename": "zh_TW.json"
    },
    {
        "language": "en_US",
        "name": "English",
        "filename": "en_US.json",
        "iconFile": "en_US.png"
    }
]
```
language （必填）语言代码，必须是唯一的不能与其它语言相同。
name       （可选）显示文本。如果没有设置名称，将显示语言代码。
filename （必填）语言文件
iconFile   （可选）语言图标。AYASpace 为一些国家内置了语言图标。如果您的国家/地区不可用，您可以设置此选项。

内置语言图标包括：`zh_CN` / `zh_TW` / `en_US` / `fr_FR` / `it_IT` / `ja_JP` / `ko_KR` / `pl_PL` / `ru_RU`



语言文件添加及修改注意事项：

1.  语言值必须使用前后必须使用 `"` 双引号 符号，如果语言包含 `"` 符号需要在前面加上 ` \ ` 转义，或者改用 `'` 单引号。
2.  `{xxx}` 为变量值不可以修改，例如：`{function}` `{name}` `{type}`。
