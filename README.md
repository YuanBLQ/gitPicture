# GitHub 的图床 repo

# 使用方式
1. 下载 [picGo](https://github.com/Molunerfinn/picgo/releases)
2. 配置 picGo 的 GitHub 图床信息
    
    2.1. 创建一个 public 的 repo
    
    2.2. 专门创建一个给 picGo 的 GitHub token（scopes 只需要 repo 权限就行了）
![创建 GitHub token](https://raw.githubusercontent.com/YuanBLQ/gitPicture/master/img/202109221258738.png)

    2.3. 设置 picGo 的 GitHub 图床配置
![picGo GitHub 图床配置](https://raw.githubusercontent.com/YuanBLQ/gitPicture/master/img/202109221259390.png)

3. 尽情享用

# 其他说明
由于 picGo 的图片同步功能由于[软件架构的原因](https://github.com/Molunerfinn/PicGo/issues/641)无法本身自带，picGo 纯粹用作图片上传工具。

如果要管理图片的话，可以把本 repo pull 到本地，然后用专门的图片浏览工具进行管理。

# 博客系统编辑逻辑
- 在线系统：语雀编辑（主要是为了防止图片重复修改导致污染图床/增加图床的管理成本）。
- 本地编辑：以 markdown 格式导出语雀编辑的文档，然后截图把里面的图片上传到图床（通过 iCloud/坚果云 实现多端同步）。
- 其他博客：本地 markdown 复制到对应的博客系统即可发布。