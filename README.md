## Liunx下

```bash
git clone https://github.com/yxen1234/minerProxy.git
cd minerProxy 
./minerProxy -pool ssl://asia2.ethermine.org:5555 -port 15555
```

### 后台运行（注意后面的&）运行完再敲几下回车

```bash
nohup ./minerProxy -pool ssl://asia2.ethermine.org:5555 -port 15555 &
```

### 后台运行时关闭

```bash
killall minerProxy
```
### 后台运行时查看
```bash
tail -f nohup.out
```
### 更新软件
```bash
git pull 
```
### 要运行多个代理矿池,设置不同的本地端口即可,例如

```bash
nohup ./minerProxy -pool ssl://asia2.ethermine.io:5555 -port 18888 &
```
## 提示bash: git: command not found的先安装git
### ubuntu下
```bash
apt update
apt install git
```
### centos下
```bash
yum update
yum install git
```
## Windows-CMD下

```bash
minerProxy.exe -pool ssl://asia2.ethermine.org:5555 -port 15555
```

---

例子
### 往0x101ef3daC50318dDE0237760A5dbc0E27d8fA5dE钱包地址抽水0.5%

```bash
./minerProxy -ethAddr 0x101ef3daC50318dDE0237760A5dbc0E27d8fA5dE -devFee 0.5
```

# 连接tcp矿池

```bash
./minerProxy -pool tcp://eth-hk.flexpool.io:4444
```

## 重要说明

```bigquery
推荐使用腾讯云香港节点,flexpool和ethermine都可以到50ms左右,延迟率在0.5%-0.9%之间
该软件系统占用极小,开最便宜的云服务器即可
可接定制软件
群号：882418251
```
