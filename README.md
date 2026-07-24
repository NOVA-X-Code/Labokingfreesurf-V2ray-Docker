# 🚀 Labokingfreesurf Simple V2Ray Service

![Docker Pulls](https://shields.io)
![Docker Image Size](https://shields.io)
![Docker Hub](https://img.shields.io/badge/Docker-Hub-2496ED?logo=docker)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📦 Docker Image Available on Docker Hub

This image is publicly available on Docker Hub:

```bash
docker pull labokingfreesurf/labokingfreesurf-gcp:latest
```

👉 [View on Docker Hub](https://docker.com)

## ✨ Features
```text
| Feature                | Status                                  |
| :----------------------|-----------------------------------------|
| 🔵 VMess Protocol      | ✅ Active                              |
| 🟢 VLESS Protocol      | ✅ Active                              |
| 🟡 Trojan Protocol     | ✅ Active                              |
| 🌐 WebSocket Transport | ✅ Enabled                             |
| 🔒 TLS Encryption      | ✅ Automatic (Cloud Run)               |
| 🎨 Web Interface       | ✅ Included                            |
| 🔗 Link Generator      | ✅ `vmess://`, `vless://`, `trojan://` |
| 📱 Mobile Friendly      | ✅ Responsive Design                   |
| 🚀 service Ready       | ✅ GCP Cloud Run Compatible            |
```

## 🚀 Quick Start

### Run with Docker

```bash
docker run -d -p 8080:8080 --name v2ray-gcp labokingfreesurf/labokingfreesurf-gcp:latest
```

### Check if it's working

```bash
docker ps
docker logs v2ray-gcp
```

### Open the Web Interface

Open your browser and navigate to: `http://localhost:8080 or web url`

---

## 🐳 Docker Compose

Create a `docker-compose.yml` file:

```yaml
version: '3.8'

services:
  v2ray:
    image: labokingfreesurf/labokingfreesurf-gcp:latest
    container_name: labokingfreesurf-gcp
    ports:
      - "8080:8080"
    restart: unless-stopped
```

Then run the following command to start the container:

```bash
docker-compose up -d
```

---

## 🔌 Protocols Configuration

This image runs three active protocols simultaneously:
```text
| Protocol  | Path                                                  | Port| TLS |
| : ------- | :---------------------------------------------------  |:---:|:---:|
| 🔵 VMess | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/vmess`   | 443 | ✅ |
| 🟢 VLESS | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/vless`   | 443 | ✅ |
| 🟡 Trojan | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/trojan` | 443 | ✅ |
```
### Client Configuration Details
```text
| Parameter     | VMess                | VLESS                | Trojan               |
| :----------   | :------------------- | :------------------- | :------------------- |
| Address       | Your service Run URL | Your service Run URL | Your service Run URL |
| Port          | 443                  | 443                  | 443                  |
| UUID/Password | `ccc22-uuid-1111-aaaa-aaaaaaaaaaa1` | `aaa11-uuid-2222-bbbb-bbbbbbbbbbb2` | `@Labokingfreesurf` |
| Network       | ws | ws | ws |
| Path          | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/vmess` | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/vless` | `/@Labokingfreesurf/@hat_tunnel/@Dr_internet4/trojan` |
| TLS           | ✅ Enabled | ✅ Enabled | ✅ Enabled |
| Security      | none       | none        | none        |
```
---

## 🔐 Security
```text
| Security Measure          | Status                                  |
| :------------------------ | :---------------------------------------|
| **TLS/SSL Encryption**    | ✅ Provided automatically by Cloud Run  |
| **Client Authentication** | ✅ UUID / Password Required             |
| **Transport Security**    | ✅ TLS 1.2+ Enforced                    |
| **Web Interface**         | ✅ Public (with secure link generation) |
```
All connections are fully encrypted and secure.

---

## 📚 How It Works

1. **Access**: User opens the web interface (via your deployed Cloud Run URL).
2. **Selection**: User selects a protocol (**VMess**, **VLESS**, or **Trojan**).
3. **Generation**: Clicks on **"Generate Link"**.
4. **Copy**: Copies the generated connection string (`vmess://`, `vless://`, or `trojan://`).
5. **Import**: Imports the link into a V2Ray client (*v2rayN, Nekoray, Shadowrocket*, etc.).
6. **Connect**: Connects securely through your proxy.

---

## 🛡️ Acceptable Use Policy

This service is intended for legitimate purposes only:
* 🔒 Securing your internet connection.
* 🏢 Establishing secure remote work environments.
* 🌐 Accessing geo-restricted resources legally.
* 🔐 Protecting online personal privacy.

> ⚠️ **WARNING**: This service must **NOT** be used for illegal activities, copyright infringement, bypassing local laws, or any form of malicious network abuse. Users are solely responsible for their activities.

---

## 🌍 Join and Support NOSTRA Community

### Official Channels


| Platform | Link / Button |
| :--- | :--- |
| 💬 **Discord** | [![Discord](https://shields.io)](https://discord.gg/xGAGs69UHj) |
| 📢 **WhatsApp Official** | [![WhatsApp Official](https://shields.io)](https://whatsapp.com/channel/0029Vb8ZJnsAYlUHo1uA6W0y) |
| 📢 **WhatsApp Laboking** | [![WhatsApp Laboking](https://shields.io)](https://whatsapp.com/channel/0029Vb6yLAG9WtC0zbXeEo2t) |
| 👥 **WhatsApp Community** | [![WhatsApp Community](https://shields.io)](https://chat.whatsapp.com/LUkXjJNfWrT8Fz7akxosH0) |
| 📢 **Telegram Group 1** | [![Telegram Group 1](https://shields.io)](https://t.me/LaboKingFreeSurf) |
| 📢 **Telegram Group 2** | [![Telegram Group 2](https://shields.io)](https://t.me/hat_tunnel) |


<div>© 2026 Labokingfreesurf GCP | Powered by NOSTRA</div>
