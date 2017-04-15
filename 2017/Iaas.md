## IaaS 基础设施

> 为小团队打造一个经济实惠 IaaS, 主要解决：1内网各类服务不稳定，2开发资源严重缺乏。
小团队穷，但再穷也不能穷基础


### 虚拟化主机：Vagrant
宿主机为 centOS 6.7（为PC机安装系统这步怎么也少不了，交给运维网管）
虚拟化主机为 virtualBox + Vagrant (免费，配置式的，跟 docker 可打包，可搬运)

*** 网络配置 ***

利用shell来配置网络
```
Vagrant.configure("2") do |config|
  config.vm.network "public_network", auto_config: false

  # manual ip
  config.vm.provision "shell",
    run: "always",
    inline: "ifconfig eth1 192.168.0.17 netmask 255.255.255.0 up"
end
```


### 私有云： zstack

** 优点 **
- 基于 kvm，虚拟机性能最高
- 拥有简单的云控制台
- 开源，有免费版（部分功能受限，但不影响）
