# Windows docker 设置

- ### 配置加速

  - 阿里云加速

    > 针对安装了 Docker for Windows 的用户，您可以参考以下配置步骤：
    >在系统右下角托盘图标内右键菜单选择 Settings，打开配置窗口后左侧导航菜单选择 Docker Daemon。编辑窗口内的 JSON 串，填写下方加速器地址：
    >
    >```
    >{
    >  "registry-mirrors": ["https://some-string.mirror.aliyuncs.com"]
    >}
    >```
    >
    >   编辑完成后点击 Apply 保存按钮，等待 Docker 重启并应用配置的镜像加速器。

  - Docker 中国官方镜像加速

    > 您可以使用以下命令直接从该镜像加速地址进行拉取：
    >
    > ```
    > $ docker pull registry.docker-cn.com/myname/myrepo:mytag
    > ```
    >
    > 例如:
    >
    > ```
    > $ docker pull registry.docker-cn.com/library/ubuntu:16.04
    > ```