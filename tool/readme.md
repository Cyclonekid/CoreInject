# 🛠️ 工具目录说明

本目录包含了 CoreInject 项目的各种实用工具和脚本。

---

## 📁 工具列表

### 🔧 核心工具

| 工具名称 | 描述 | 状态 |
|---------|------|------|
| **insert_dylib** | 动态库注入工具 | ✅ 可用 |
| **optool** | iOS 二进制文件操作工具 | ✅ 可用 |
| **GenShineImpactStarter** | 原神启动器，用于IPA注入 | ✅ 可用 |

### 🎮 启动脚本

| 脚本名称 | 描述 | 平台 |
|---------|------|------|
| **Crossover Activation Script.command** | Crossover 激活脚本 | macOS |
| **KeygenStarter** | 密钥生成器启动器 | macOS |

### 🌐 其他工具

| 工具名称 | 描述 | 状态 |
|---------|------|------|
| **EmbyServerUbuntuCrack** | Emby服务器破解工具 | ✅ 可用 |
| **termius_zh_CN** | Termius 中文本地化 | ✅ 可用 |

---

## 🚀 使用方法

### 1. 设置执行权限

```bash
# 为所有脚本设置执行权限
chmod +x *.command
chmod +x GenShineImpactStarter
chmod +x insert_dylib
chmod +x optool
```

### 2. 使用原神启动器

```bash
# 注入IPA文件
./GenShineImpactStarter packipa "ipa文件路径" ./CoreInject.dylib
```

### 3. 使用动态库注入工具

```bash
# 注入动态库到二进制文件
./insert_dylib "动态库路径" "目标二进制文件"
```

---

## 📱 平台兼容性

- ✅ **macOS 10.13+**
- ✅ **iOS 12.0+** (通过IPA注入)
- 🔄 **Linux** (部分工具)

---

## ⚠️ 注意事项

1. **权限设置**: 确保工具具有适当的执行权限
2. **路径正确**: 使用绝对路径或正确的相对路径
3. **版本兼容**: 确保工具版本与目标系统兼容
4. **备份数据**: 操作前请备份重要文件

---

## 🔗 相关链接

- [主项目README](../readme.md)
- [iOS注入指南](../iOSHijack/readme.md)
- [使用文档](https://qiuchenlyopensource.github.io/Documentaions/)

---

<div align="center">

**🛠️ 工具在手，天下我有！**  
**🚀 让注入变得简单！**

</div>
