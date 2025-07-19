# Notion Widget Test

这是一个可以嵌入 Notion 的测试 Widget，已优化为完全兼容 Notion 的嵌入机制。

## 功能特性

- ✅ 支持嵌入 Notion 页面（已修复兼容性问题）
- 🎯 固定高度设计，避免 DOM 冲突
- 📱 响应式设计
- 🎨 简洁美观的界面
- 🔄 使用 postMessage 通信（更安全）

## 最新更新 (修复 Notion 错误)

### 问题解决

- ❌ 移除了导致 Notion DOM 冲突的 iframe-resizer 库
- ✅ 使用固定高度 (120px) 替代动态调整
- ✅ 采用 postMessage API 进行安全的父子页面通信
- ✅ 优化 CSS 样式，确保在 Notion 中完美显示

### 技术改进

- 使用现代字体栈 (-apple-system, BlinkMacSystemFont 等)
- 添加悬停效果和过渡动画
- 改善响应式布局
- 透明背景，更好融入 Notion 页面

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
3. Widget 会以固定高度 (120px) 显示，不会触发 DOM 冲突

## 技术栈

- HTML5
- CSS3（现代 Flexbox 布局）
- 原生 JavaScript（postMessage API）

## 兼容性说明

- ✅ **完全兼容 Notion 嵌入机制**
- ✅ 不会触发 Notion 的 DOM 变更警告
- ✅ 支持 HTTPS（Notion 要求）
- ✅ 跨浏览器兼容
- ✅ 移动端友好

## 故障排除

如果在 Notion 中遇到问题：

1. 确保使用 HTTPS URL
2. 检查网络连接
3. 刷新 Notion 页面重新加载 Widget
