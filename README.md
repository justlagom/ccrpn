-----
# 🚀 ClawCloud Run - ENC+Vioion-Xhttp-ARGO 代理节点

[](https://github.com/justlagom/ccrpn)
[](https://www.google.com/search?q=https://app.koyeb.com/deploy%3Fname%3Dkoyebne%26type%3Dgit%26repository%3Dgithub.com/justlagom/koyebne%26branch%3Dmain%26env%5BENC_CONFIG%5D%3D)

一个部署在 [ClawCloud Run Platform](https://www.koyeb.com/) 上的 **ENC+Vioion-Xhttp** 代理节点项目，旨在提供一个稳定、快速的代理服务。


## ✨ 主要特性

  * **多协议支持:** 集成了 **ENC**、**Vioion**、**Xhttp** 和 **ARGO** 代理协议。
  * **平台稳定:** 部署在 ClawCloud 平台，享受其高性能和全球边缘网络。


## ⚙️ 部署指南 

### 步骤 1: 准备环境变量

## ccrpn/app/xy/config.json-可选择手搓其他xray配置

## 节点参考模板： ##

**vless://%E8%87%AA%E5%AE%9A%E4%B9%89UUID@优选ip:443?encryption=mlkem768x25519plus.native.0rtt.fRLKjkBNx1N6ceiqcqilb46WNj4yvl4SgXklAFkvNhE&flow=xtls-rprx-vision&security=tls&sni=%E5%9B%BA%E5%AE%9A%E9%9A%A7%E9%81%93&fp=chrome&alpn=h2&insecure=0&allowInsecure=0&type=xhttp&path=%E8%87%AA%E5%AE%9A%E4%B9%89%E8%B7%AF%E5%BE%84&mode=auto#ENC%2BVision-Xhttp-ARGO**

## 在部署到 ClawCloud 之前，您需要设置核心的代理配置参数**uuid**、**path**，也可手搓更改xray配置文件。 ##

| 变量名 | 描述 | 示例值 |
| :--- | :--- | :--- |
| **`CLOUDFLARED_TOKEN`** | 必备 | `设置cf tunel时获取token（镜像默认localhost:8001）` |
| **`UUID`** | 自定义uuid-必需 | `5936acb6-e65e-4631-bedf-ce723a1a375d` |
| **`PROXY_PATH`** | 自定义path-必需 | `/5936acb6` |
| **`DOMAIN`** | 容器域名(首次部署后可见)-必需 | `xxx.xxx.com` |

-----

## 🛠️ 本地开发与测试

如果您需要本地测试，请确保您已安装 Docker 环境：

```bash
# 克隆项目
git clone https://github.com/justlagom/hfne.git
cd hfne

# (可选) 在本地创建一个 .env 文件来设置您的 ENC_CONFIG

# 构建 Docker 镜像
docker build -t hfne:latest .

# 运行容器 (替换为您的配置)
docker run -d -p 8080:8080 \
  -e ENC_CONFIG='{"uuid": "your-uuid", "path": "/testpath", "port": 8080}' \
  hfne:latest
```

## 📄 License

该项目基于 **MIT License** 发布。

-----

希望这份 README 能够清晰地展示您的项目！
