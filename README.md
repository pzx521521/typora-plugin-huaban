# [HuabanBatchUpload] golang版本
花瓣网图片批量上传工具
[python版本的](https://github.com/Pingze-github/HuabanBatchUpload)这个太老了 已经不能用了,现在全部是V3接口
## 功能说明
这是一个用于向花瓣网批量上传/下载 图片的程序。
+ 多线程并发，可以快速上传大量文件
+ 自动传输错误重试
## 比较
|          | 跨域 | 网页直接使用 | 不压缩          |
|----------|---|--------|--------------|
| bilibili | ✅ | ❌(需要no-referrer)  | ❌(部分压缩机制不知道) |
| huaban   | ❌ | ✅      | ✅            |
## 获取可执行版方法
[github-release](https://github.com/pzx21521/HuabanBatchUpload/releases)

## 使用方法 1
`config.json`配置 **用户名 密码 画板名**,

```json
{
  "name": "your_account",
  "pass": "your_password",
  "board": "your_board"
}
```
把文件/文件夹 拖上去就好, 或者在命令行中执行：`huaban /path/to/images`
## 使用方法 2
`config.json`配置好 **用户名 密码 画板名** 和 文件/文件夹
```json
{
  "name": "your_account",
  "pass": "your_password",
  "board": "your_board",
  "dir": ["/Users/parapeng/Downloads", "./upload.gif"],
  "debug": true
}
```
运行就好

## 使用方法 3
在命令行中执行：`huaban -name=your_account -pass=your_password -board=your_board -dir=/path/to/images -debug=true`

## typora使用
`config.json`配置好 **用户名 密码 画板名** **不要**配置debug
```json
{
  "name": "your_account",
  "pass": "your_password",
  "board": "your_board"
}
```
### 可以直接复制粘贴/拖上来

![output](https://gd-hbimg.huaban.com/1c528e76c82479b818d39069980c7a5d1743e96f5797f-8iQEPg)

### 可以输入链接后上传

![upload](https://gd-hbimg.huaban.com/e5c68d00cad1add003e94fbc42426100403f3e6f1187a7-dJC6l9)
可以直接copy,paste

### typora免费版下载
- [Windows](https://typora.io/windows/dev_release.html)
- [windows x64 国内OSS镜像下载](https://jiali0126.oss-cn-shenzhen.aliyuncs.com/typora/typora-update-x64-1117.exe)
- [Mac](https://typora.io/dev_release.html)

