# KARAS_Jekyll



## About

KARAS is lightweight markup language. And this is the plugin to use KARAS in Jekyll.
If you want to get more info about KARAS, please visit [lightweightmarkuplanguage.com](http://lightweightmarkuplanguage.com).



## How to Use

This Jekyll plugin acts as // Converter //. Unzip download file, and put each files into ``` _plugins ``` directory. There is no need to change the any other settings. Text file with the extension ```. karas ``` will be converted to an HTML page.



### Problem

KARAS for Jekyll has one important problem. Jekyll has a template engine // Liquid //, and the syntax conflicts with Block group syntax of KARAS. Even if the results of converted KARAS text not include ``` {{ ``` Symbol, Liquid throws Exception. Because this problem can not be corrected from the plugin, Block group syntax in KARAS for Jekyll is slightly modified.

In order to write the Block group in KARAS for Jekyll, use ``` {\\{ ``` and ``` {\\{ ```,  insted of ``` {{ ``` and ``` }} ```. Unfortunately, this would detract from the beauty of KARAS. However, I could not find any other way.



## System requirements

Need Ruby version 1.9 or later.



## License

KARAS and the converters are licensed under BSD.
KARAS for Jekyll is licensed under BSD.