#qiniu_sync

基于七牛Python SDK写的一个同步脚本。
支持批量比较文件，差异增量更新、批量更新。
然后生成MarkDown的插图地址到 `md_url.txt`

## 使用方式

* 安装七牛Python SDK
`pip install qiniu`

* 填写脚本文件(qiniusync.py)的配置信息
```
access_key = ''
secret_key = ''
bucket_name = ''
bucket_domain = ''
```
>注册后可以拿到对应的信息 

* 将脚本文件(qiniusync.py)拷贝到待同步根目录

* 运行脚本
```
python qiniusync.py
python qiniusync.py down
python qiniusync.py down [文件路径前缀]
```
