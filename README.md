# 简单创建一个可以使用ipv6的shadowsocks

## 在构建服务器时，需要添加勾选ipv6
- ![avatar](/img/a.png)
***

## 选择服务器类型
- 依次执行以下代码： cd ../etc/shadowsocks  vi server.json，编辑server.json文件
- ![avatar](/img/b.png)
- ![avatar](/img/c.png)
- 输入 i ，将server.json的server字段的值:"0,0,0,0"改为 "::"，并修改你想要的端口和密码（不要使用默认密码），按 Esc 退出编辑模式，输入 :wq ，保存退出。
- 最后输入  ssserver -c /etc/shadowsocks/server.json -d start &  启动shadowsocks。
***

## 查看你的ipv6地址
- 可以从vultr官网中获取。
- ![avatar](/img/d.png)
- ![avatar](/img/e.png)
- 也可以输入 ifconfig 获取。
- ![avatar](/img/f.png)
***
