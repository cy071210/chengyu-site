# 程雨 · 个人主页

这是程雨的个人主页项目，包含自我介绍、可联网搜索和反馈功能。

## 文件说明

- `index.html` — 单页静态站点，包含：
  - 个人简介（姓名、学校、个人一句话介绍、邮箱联系方式）
  - 联网搜索区域（支持切换多个搜索引擎）
  - 反馈表单（通过 Web3Forms 投递到 `hellsing_2024@qq.com`）

## 本地预览

直接用浏览器打开 `index.html`，或在该目录运行一个静态服务器：

```bash
# Python
python -m http.server 8080
# Node
npx serve .
```

访问 http://localhost:8080

## 部署到 GitHub Pages

1. 把本目录推送到 GitHub 仓库（默认分支 `main`）。
2. 在仓库页面 → Settings → Pages → Build and deployment → Source 选择 `Deploy from a branch`，Branch 选择 `main`，目录 `/ (root)`。
3. 等待几分钟，访问 `https://<你的GitHub用户名>.github.io/<仓库名>/`。

## 关于反馈表单

页面里的 Web3Forms `access_key` 是公开的（前端静态网页无法保密）。如需更换：

1. 登录 https://web3forms.com 生成新的 Access Key。
2. 打开 `index.html`，搜索 `access_key`，把 value 替换为新 Key。

或使用其它第三方表单服务（Formspree、Getform 等）。
