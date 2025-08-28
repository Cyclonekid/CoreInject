# 🎬 Emby Server Ubuntu 破解版

> 🚀 **自用 Emby Server 破解版本**
> 
> 支持硬件解码和服务器验证绕过

---

## 🚀 快速开始

### 1. 修改映射目录
根据你的需求修改 `docker-compose.yml` 中的目录映射

### 2. 启动服务
```bash
docker compose up -d
```

---

## 📋 版本信息

| 组件 | 版本 | 说明 |
|------|------|------|
| **Emby Server** | 4.9.0.23 | 官方版本 |
| **Docker** | 最新 | 容器化部署 |

---

## ⚠️ 重要注意事项

### 配置持久化
1. **保留配置**: `docker compose down` 不会删除配置信息
2. **完全清理**: 如需删除配置，使用 `docker compose down -v`
3. **更新方式**: `docker compose down && docker compose up -d`

---

## 🔧 破解原理

### 1. 硬件解码破解
**目标**: `Emby.Server.Implementations.Security.RegRecord::get_registered()`

**修改内容**:
```csharp
// 原始代码
bool get_registered() {
    // ... 验证逻辑
    return false;
}

// 破解后
bool get_registered() {
    // ... 验证逻辑
    return true;  // 修改这一字节
}
```

### 2. 服务器验证绕过
**技术**: 前端 JS 层 Hook 拦截 HTTP 页面请求

> 💡 **注意**: 此技术涉及较深的逆向工程知识，不建议新手研究

---

## 🐳 Docker 部署

### 环境要求
- Ubuntu 18.04+
- Docker 20.10+
- Docker Compose 2.0+

### 部署步骤
```bash
# 1. 克隆项目
git clone <repository_url>
cd EmbyServerUbuntuCrack

# 2. 修改配置
vim docker-compose.yml

# 3. 启动服务
docker compose up -d

# 4. 查看状态
docker compose ps
```

---

## 📁 文件结构

```
EmbyServerUbuntuCrack/
├── docker-compose.yml      # Docker 编排文件
├── apploader.js           # 应用加载器
├── Emby.Server.Implementations.dll  # 破解后的核心库
└── readme.md              # 说明文档
```

---

## 🔒 安全提醒

> ⚠️ **重要**: 本工具仅供学习和研究使用
> 
> - 请遵守当地法律法规
> - 仅用于个人学习和研究
> - 不得用于商业用途
> - 使用前请备份重要数据

---

## 📞 技术支持

如遇到问题，请：
1. 检查 Docker 环境
2. 查看容器日志
3. 确认端口配置
4. 验证文件权限

---

<div align="center">

**🎬 Emby 破解成功！**  
**🚀 享受无限流媒体体验！**

</div>

---

## 📝 备注

> 💭 **个人观点**: 
> 
> 破解一个毫无安全意识的应用程序，把网上不少贵物小学生得瑟的那样，发个版本到处装大神，你装你吗呢？菜鸟。

*—— QiuChenly*