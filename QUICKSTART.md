# 🚀 快速开始指南

欢迎使用 QwenImg！本指南将帮助你快速搭建环境并开始创作。

## 1. 一键安装

我们提供了一个自动化脚本，可以一次性完成所有配置。

**Linux / macOS:**

```bash
# 1. 赋予脚本执行权限
chmod +x install.sh

# 2. 运行安装脚本
./install.sh
```

脚本会自动：
- ✅ 检查系统环境
- ✅ 创建 Python 虚拟环境
- ✅ 安装后端依赖
- ✅ 安装前端依赖
- ✅ 配置环境变量
- ✅ 恢复示例数据

## 2. 配置 API Key

安装完成后，你需要配置阿里云 DashScope API Key。

1. 打开项目根目录下的 `.env` 文件。
2. 填入你的 API Key：

```env
DASHSCOPE_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

> 还没有 API Key？[点击这里获取](https://help.aliyun.com/zh/model-studio/get-api-key)

## 3. 启动服务

使用启动脚本同时启动前端和后端服务：

```bash
./start_dev.sh
```

启动成功后，访问：
- **Web 界面**: [http://localhost:3000](http://localhost:3000)
- **API 文档**: [http://localhost:8000/docs](http://localhost:8000/docs)

## 4. 开始创作

### 文生图
1. 在输入框输入提示词（例如："一只在太空漫步的猫"）。
2. 点击 **"生成"** 按钮。
3. 等待几秒钟，图片将出现在下方画廊中。

### 图生视频
1. 将生成的图片拖入 "图生视频" 区域，或点击上传图片。
2. 输入动作描述（可选）。
3. 点击 **"生成视频"**。

## 常见问题

**Q: 安装脚本报错 "Permission denied"？**
A: 请确保运行了 `chmod +x install.sh`。

**Q: 启动后浏览器无法访问？**
A: 请检查终端是否有报错信息，确认端口 5173 (前端) 和 8000 (后端) 未被占用。

**Q: 生成图片失败？**
A: 请检查 `.env` 文件中的 API Key 是否正确，以及网络连接是否正常。

---
更多详细信息，请参阅 [README.md](./README.md)。
