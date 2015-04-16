# Linux配置教程

`注：未经说明情况下，均以Ubuntu作为默认Linux发行版本，由于MAC下已经有优秀的图形化界面，所以这里的Ubuntu指去掉图形化界面的Ubuntu`

### bash
    交互登陆Shell（通过bash --login登录，logout登出），bash执行时先执行/etc/profile文件夹，再执行~/.bash_profile、~/.bash_login和~/.profile中从左往右第一个找到的可读文件，结束时执行~/.bash_logout文件

    交互非登陆式Shell（我们在图形界面启动Shell就是这种方式），此时bash启动只执行~/.bashrc（修改的重要文件），所以我们修改一般只修改这个文件（修改环境变量、命令等）

    非交互式Shell（即执行shell脚本的时候），bash执行时继承了对应交互式的配置文件




### virtualbox（这里Linux作为虚拟机）
    sudo mount -t vboxsf virtualboxFolderName mountLocation：挂在共享文件夹



### 启动
    /boot/grub/grub.conf：开始的选择菜单配置文件
    /etc/rc.local：系统启动自动运行脚本
    /etc/fstab：自动挂载的设置文件
    /etc/rc.local：自动挂载文件
    /etc/shells：存储有哪些shell
    /etc/passwd：记录登录名与UID匹配的文件
    /etc/shadow：保存关于用户的一些记录



### 其它
    /etc/apt/sources.list：apt源文件
