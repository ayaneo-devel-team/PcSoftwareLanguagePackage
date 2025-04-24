​	If the current AYASpace language does not include your country, you can also add the language file and modify the configuration file `config.json` in the AYASpace installation directory/language folder, or modify the existing language file (please note that AYASpace upgrade may overwrite it, so you need to backup the file before upgrading).



`config.json` can be configured to display in AYASpace settings/general/language list

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
language       (required)  Language code must be unique and cannot be the same as other languages.
name             (optional)  displays text. If no name is set, the language code will be displayed.
filename        (required)  Language file
iconFile          (optional)  language icon. AYASpace has built-in language icons for some countries.  If it is not available in your country/region, you can set this option.



The built-in language icons include: `zh_CN` / `zh_TW` / `en_US` / `fr_FR` / `it_IT` / `ja_JP` / `ko_KR` / `pl_PL` / `ru_RU`



Precautions for adding and modifying language files:

1. Language values must use double quotation marks before and after, and if the language contains a `"` symbol, it needs to be escaped with a `\ ` symbol in front, or use single quotation marks instead.
2. `{xxx}` is a variable value that cannot be modified, for example: `{function}` `{name}` `{type}`.

