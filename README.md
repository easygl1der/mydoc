# 研究文档库

这是一个用于展示和分享PDF研究文档的静态网站，托管在GitHub Pages上。

## 📚 包含的文档

1. GARCH Ito IV Presentation (2025-06-08)
2. GARCH Ito IV Presentation (2025-04-26)
3. GARCH LSTM IV (2025-11-02)
4. Mathematica项目 - 23363017 - 乐绎华

## 🚀 部署到GitHub Pages

### 步骤1：创建GitHub仓库

1. 登录GitHub账户
2. 点击右上角的 `+` 按钮，选择 `New repository`
3. 输入仓库名称（例如：`research-pdfs`）
4. 选择 `Public`（公开仓库）
5. 点击 `Create repository`

### 步骤2：上传文件

#### 方法A：通过Git命令行

```bash
# 初始化Git仓库
git init

# 添加所有文件
git add .

# 提交更改
git commit -m "Initial commit: Add PDF library website"

# 添加远程仓库（替换为你的GitHub仓库地址）
git remote add origin https://github.com/你的用户名/你的仓库名.git

# 推送到GitHub
git branch -M main
git push -u origin main
```

#### 方法B：通过GitHub网页界面

1. 进入你创建的仓库
2. 点击 `Add file` -> `Upload files`
3. 将以下文件拖拽上传：
   - `index.html`
   - 所有PDF文件（4个）
   - `README.md`
4. 点击 `Commit changes`

### 步骤3：启用GitHub Pages

1. 进入仓库的 `Settings` 页面
2. 在左侧菜单找到 `Pages`
3. 在 `Source` 部分，选择 `main` 分支
4. 点击 `Save`
5. 等待几分钟后，你的网站就会上线

### 步骤4：访问你的网站

网站地址格式为：`https://你的用户名.github.io/你的仓库名/`

例如：`https://username.github.io/research-pdfs/`

## 💡 功能特点

- ✨ 现代化、响应式设计
- 📱 移动端友好
- 🎨 渐变色背景和卡片式布局
- 👁️ 在线预览PDF（在浏览器新标签页中打开）
- 💾 一键下载功能
- 🌐 无需服务器，完全静态托管

## 🔧 自定义修改

### 添加更多PDF

1. 将PDF文件上传到仓库
2. 在 `index.html` 中的 `<div class="pdf-grid">` 部分添加新的卡片：

```html
<div class="pdf-card">
    <div class="pdf-icon">📄</div>
    <div class="pdf-title">你的PDF标题</div>
    <div class="pdf-actions">
        <a href="你的文件名.pdf" class="btn btn-primary" target="_blank">在线预览</a>
        <a href="你的文件名.pdf" class="btn btn-secondary" download>下载</a>
    </div>
</div>
```

### 修改样式

所有样式都在 `<style>` 标签中，你可以：
- 修改颜色渐变（`background: linear-gradient(...)`）
- 调整卡片大小（`grid-template-columns`）
- 更改字体和间距

## 📝 注意事项

- PDF文件名中包含中文字符时，确保文件编码正确
- GitHub Pages有仓库大小限制（建议单个仓库不超过1GB）
- 大型PDF文件可能加载较慢，建议优化PDF大小

## 📄 许可证

MIT License

---

如有问题或建议，欢迎提Issue！

