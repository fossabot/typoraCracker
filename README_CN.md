# typora Cracker

一个typora的Patch和KeyGen工具

## 敬告
```
仅供学习和讨论，请不要从事任何非法行为。
由此产生的任何问题都将由用户（您）承担。
```

## Features

- 理论上支持Typora支持的所有操作系统

## 食用方式

1. `pip install -r requirements.txt`
2. `python typora.py --help`
3. 阅读帮助文档及使用。
4. 修改导出的 License.js。
5. 替换原目录下的 app.asar。
6. 运行KeyGen程序。
7. 正常激活。


## 示例

```shell
> python typora.py --help
usage: typora.py [-h] [-u] [-f] asarPath dirPath

[extract and decryption / pack and encryption] app.asar file from [Typora].

positional arguments:
  asarPath    app.asar file path/dir [input/ouput]
  dirPath     as tmp and out directory.

optional arguments:
  -h, --help  show this help message and exit
  -u          pack & encryption (default: extract & decryption)
  -f          enabled prettify/compress (default: disabled)

If you have any questions, please contact [ MasonShi@88.com ]

> python typora.py {installRoot}/Typora/resources/app.asar workstation/outfile/
⋯
> python typora.py -u workstation/outfile/ workstation/outappasar
⋯
> cp {installRoot}/Typora/resources/app.asar {installRoot}/Typora/resources/app.asar.bak
> mv workstation/outappasar/app.asar {installRoot}/Typora/resources/app.asar
# (patch code)
> node keygen.js
XXXXXX-XXXXXX-XXXXXX-XXXXXX
> typora
# (input info)
email: crack@example.com
serial: XXXXXX-XXXXXX-XXXXXX-XXXXXX
```

## LICENSE
 MIT LICENSE
