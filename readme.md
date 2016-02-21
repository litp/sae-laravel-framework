# Laravel Framework (Kernel) For SAE

Laravel Framework for SAE 是一个修改过的，可以在SAE上完美运行的Laravel版本。

## 代码修改更改处

1. 适配putenv被禁用

SAE禁用了putenv函数（其他很多开发平台也同样会禁用putenv），Laravel中使用的phpdotenv模块不能正常使用。

Laravel Framework for SAE使用sae-phpdotenv替代phpdotenv，并修改env()函数使其从全局变量$_ENV中获取变量，从而使phpdotenv可以在SAE中正常使用。

2. Todo


另外，欢迎提供各种意见及建议。