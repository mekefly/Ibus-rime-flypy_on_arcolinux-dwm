# Ibus-rime-flypy_on_arcolinux-dwm
在arcolinux-dwm上安装小鹤音形

## 1.开始安装

任选一个在命令行执行

打开命令行的按钮`win + Enter`

- 能访问github可以执行

```shell
curl https://raw.githubusercontent.com/mekefly/Ibus-rime-flypy_on_arcolinux-dwm/main/install.sh | bash
```

- 国内网络可以选择

```shell
curl https://gitee.com/mekefly/Ibus-rime-flypy_on_arcolinux-dwm/main/install.sh | bash
```

安装完成后就可以使用`ctrl + shift + d`输入 `ibus-daemon` 然后**回车**执行就可

## 2. 配置自动启动

### 2.1  找到arco-dwm的目录

执行

```shell
cd ~/.config/arco-dwm
```

### 2.2  编辑自启动文件

执行

```shell
vim ./autostart.sh
```

然后在最后面添加一行

```shell
run "ibus-daemon --xim -d" 
```



###  重启后就可以使用了

