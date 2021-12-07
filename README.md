# 项目介绍

将网易云音乐的 `.ncm` 格式转换成 `.flac` 格式和 `.mp3` 格式. 

## 需要工具

- Python3
- Crypto.Cipher 依赖包, 在命令行输入 `pip3 install pycryptodome` 安装(原安装方法 `pip3 install pycrypto` 已不可用)

## 使用方法

```bash
python3 ncmdump.py [files] ...
```

将[files]更改为文件名(需带 `.ncm` 后缀, 支持批量转换, 多个文件名间用空格分开 e.g: `python3 numdump.py a.ncm b.ncm`)

## 参数说明

* `--no-output` 取消转换进度输出
* `--all` 将目录下所有 `.ncm` 文件转换

## 更新日志

* 2021-12-07 18:32 - 增加将目录下所有 `.ncm` 文件转换的功能, 增加 `--all` 参数 
* 2021-10-15 19:17 - 增加转换进度输出, 增加`--no-output`参数
