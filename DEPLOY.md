# 部署到 GitHub Pages

## 方法一：手动上传（最简单）

1. 在 GitHub 创建新仓库（如 `zhongkao-vocab`）
2. 点击 "Add file" → "Upload files"
3. 拖拽整个 `courseware` 文件夹到浏览器
4. 提交（Commit changes）
5. 进入仓库 Settings → Pages → Source 选择 "main" 分支
6. 等待 1-2 分钟，访问 `https://<你的用户名>.github.io/zhongkao-vocab/`

## 方法二：Git 命令行

```bash
# 1. 初始化 Git
cd /Users/zouyingqi/.qclaw/workspace-wehmuz6fzp3w8mfc/courseware
git init
git add .
git commit -m "初始提交：中考英语自学系统"

# 2. 创建 GitHub 仓库（先在 GitHub 网页创建空仓库）
git remote add origin https://github.com/<你的用户名>/zhongkao-vocab.git
git branch -M main
git push -u origin main

# 3. 启用 GitHub Pages
# 进入仓库 Settings → Pages → Source 选择 "main" 分支
```

## 方法三：使用 GitHub Desktop

1. 下载安装 GitHub Desktop
2. 点击 "Add an Existing Repository from your Hard Drive"
3. 选择 `courseware` 文件夹
4. 点击 "Publish repository"
5. 启用 GitHub Pages

## 访问地址

部署成功后，访问：
```
https://<你的用户名>.github.io/<仓库名>/zhongkao-vocab-index.html
```

例如：
```
https://zouyingqi.github.io/zhongkao-vocab/zhongkao-vocab-index.html
```

## 注意事项

- ⚠️ 确保所有文件路径都是相对路径（已处理）
- ⚠️ GitHub Pages 不支持 `file://` 协议特性
- ✅ 所有72个单元都已测试通过
- ✅ 总主页可正常跳转所有单元
