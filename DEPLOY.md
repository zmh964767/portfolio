# 🚀 部署到 Netlify

## 方式一：Netlify 网页部署（推荐，最简单）

### 步骤：

1. **访问 Netlify**
   - 打开 https://app.netlify.com
   - 登录（推荐用 GitHub 登录）

2. **添加新站点**
   - 点击 "Add new site" → "Import an existing project"
   - 选择 "Deploy with GitHub"
   - 授权 Netlify 访问你的 GitHub

3. **选择仓库**
   - 找到你的 `portfolio` 或 `personal` 仓库
   - 点击选择

4. **配置构建设置**
   - **Branch to deploy**: `main`
   - **Build command**: （留空，静态网站不需要构建）
   - **Publish directory**: `/`（根目录）

5. **点击 "Deploy site"**
   - 等待 1-2 分钟
   - 部署成功后会生成一个随机域名，如 `https://xxx-xxx-xxx.netlify.app`

6. **自定义域名（可选）**
   - 进入 "Domain settings"
   - 点击 "Add custom domain"
   - 输入你的域名

---

## 方式二：Netlify CLI（需要权限）

```bash
# 安装 CLI
npm install -g netlify-cli

# 登录
netlify login

# 部署
netlify deploy --prod --dir .
```

---

## 方式三：手动上传

1. 在 Netlify 创建账号
2. 点击 "Add new site" → "Deploy manually"
3. 将整个项目文件夹拖拽到上传区域

---

## 部署后检查清单

- [ ] 网站能正常访问
- [ ] 所有链接正常工作
- [ ] 移动端响应式正常
- [ ] Dark/Light 模式切换正常
- [ ] 项目图片加载正常
- [ ] 404 页面能访问（访问不存在的 URL 测试）

---

## 环境变量（如需）

如果后续需要添加环境变量：
1. 进入 Netlify Dashboard
2. Site settings → Build & deploy → Environment
3. 添加变量

---

## 自动部署

部署后，每次 push 到 `main` 分支都会自动触发部署：

```bash
git add .
git commit -m "Update content"
git push origin main
```

Netlify 会自动检测并重新部署。
