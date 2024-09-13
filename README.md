# HyperionScan 

**HyperionScan** **(亥伯龙扫描器)**超越时间和光的泰坦神，象征扫描器速度与能力的极限。一款集资产发现和漏洞扫描于一体并支持高度自定义的分布式漏洞扫描器，旨在帮助安全人员**快速完成大批量目标的扫描任务**。

## 子系统

### 资产管理

[assertManager](https://github.com/smilexxfire/assertManager)

### 资产扫描

- [x] [子域名扫描](https://github.com/smilexxfire/SubdomainScan)（分布式）：
  - [x] subfinder
  - [x] oneforall
  - [x] amass
- [x] [域名解析](https://github.com/smilexxfire/DomainResolver)（单机）：
  - [x] dnsx：域名 -> ip
  - [x] cdncheck: 域名 -> is_cdn
  - [x] ipcheck: ip -> location、asn、is_cdn
- [x] [端口扫描](https://github.com/smilexxfire/PortScan)（分布式）：
  - [x] nmap：服务发现
  - [x] naabu：快速扫描
- [x] [站点发现](https://github.com/smilexxfire/sitefind)（分布式）：
  - [x] httpx：host:port -> url
- [x] [目录扫描](https://github.com/smilexxfire/dirscan)（分布式）：
  - [x] ffuf：url/FUZZ
  - [ ] dirsearch
- [x] [漏洞扫描](https://github.com/smilexxfire/vulnscan)（分布式）：
  - [x] nuclei：url -> vuln_info
  - [ ] xray
- [ ] 工作流支持
- [x] [云平台资源调度]()
  - [x] digitalocean
  - [ ] aws


## 部署

使用docker一键部署扫描节点



## 架构

预期设计

![](https://qiniu.xxf.world/pic/2024/09/12/344f4908-419f-43dc-a610-bd88a5ca3088.png)

工作流

![](https://qiniu.xxf.world/pic/2024/09/12/c10b3a44-e11a-4b98-90ca-a25a426710e8.png)

具体实现

![](https://qiniu.xxf.world/pic/2024/09/12/74df9648-8dee-41f3-963c-16a8a286ae67.png)
