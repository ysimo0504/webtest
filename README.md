# Notion Widget Test

这是一个可以嵌入 Notion 的测试 Widget，支持拖动缩放功能。

## 功能特性

- ✅ 支持嵌入 Notion 页面
- 🔄 支持 iframe 自动调整大小
- 📱 响应式设计
- 🎨 简洁美观的界面

## 部署说明

### Vercel 部署

1. 将项目推送到 GitHub 仓库
2. 在 Vercel 中连接 GitHub 仓库
3. Vercel 会自动识别静态 HTML 项目并进行部署
4. 部署完成后可获得公开访问链接

### 本地开发

```bash
# 安装 serve 工具（可选）
npm install -g serve

# 启动本地服务器
npm start
# 或者
serve .
```

## 在 Notion 中使用

1. 在 Notion 页面中添加 `/embed` 块
2. 粘贴部署后的 URL
3. Widget 会自动调整大小以适应内容

## 技术栈

- HTML5
- CSS3
- iframe-resizer.js（用于自动调整大小）

## 注意事项

- 确保部署后的网站支持 HTTPS（Notion 要求）
- iframe-resizer 库通过 CDN 加载，确保网络连接正常
