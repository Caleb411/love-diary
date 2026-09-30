# 恋爱日记 · 陈霖 & 文文

一份基于约会记录做成的静态纪念小站：首屏情书风、相爱天数统计、可筛选/搜索的时间线。

## 本地打开

最简单：双击 `index.html` 用浏览器打开即可。

若已安装 Node.js，也可在本目录执行：

```bash
npx --yes serve .
```

浏览器访问终端提示的地址（一般是 `http://localhost:3000`）。

Windows 也可在本目录右键「通过 Live Server 打开」（需 VS Code / Cursor 插件）。

## 目录结构

```
love-diary/
├── index.html      # 整站页面（单文件，含样式与数据）
├── SOURCE.md       # 项目原始数据（恋爱日记 Markdown）
├── package.json    # 本地预览脚本（可选）
├── vercel.json     # Vercel 部署配置（可选）
├── netlify.toml    # Netlify 部署配置（可选）
└── README.md
```

## 部署方式（任选其一）

本站是纯静态页，**发布根目录就是本文件夹**，入口为 `index.html`。

### 1. GitHub Pages（免费）

1. 新建 GitHub 仓库，把本目录推上去  
2. 仓库 **Settings → Pages**  
3. Source 选 `Deploy from a branch`  
4. Branch 选 `main`，文件夹选 `/ (root)`  
5. 保存后等待 1～2 分钟，访问：  
   `https://<用户名>.github.io/<仓库名>/`

若仓库名是 `username.github.io`，则直接访问 `https://username.github.io/`。

### 2. Vercel（推荐，拖拽或 CLI）

**网页拖拽：**

1. 打开 [https://vercel.com/new](https://vercel.com/new)  
2. 把整个 `love-diary` 文件夹拖进去  
3. 部署完成后会得到一个 `*.vercel.app` 链接  

**或 CLI：**

```bash
npx vercel
```

本目录已含 `vercel.json`，按静态站点处理。

### 3. Netlify

**拖拽：**

1. 打开 [https://app.netlify.com/drop](https://app.netlify.com/drop)  
2. 拖入 `love-diary` 文件夹  
3. 获得 `*.netlify.app` 链接  

**或关联 Git：** 导入仓库后，Publish directory 填 `.`（或留空）。

本目录已含 `netlify.toml`。

### 4. Cloudflare Pages

1. Cloudflare Dashboard → Workers & Pages → Create → Pages  
2. 连接 Git 仓库，或直接上传静态资源  
3. Build command 留空，Output directory 填 `/` 或 `.`

## 自定义

| 想改什么 | 改哪里 |
|---------|--------|
| 标题 / 名字 | `index.html` 里 `.brand`、`.hero-title` |
| 表白起始日 | 脚本里 `START_DATE`（当前为 `2025-09-13`） |
| 约会条目 | 脚本里 `diaries` 数组 |
| 配色 | `:root` CSS 变量（`--rose`、`--rose-deep` 等） |

## 说明

- 无需构建、无后端依赖  
- 字体通过 Google Fonts 加载，首次打开需联网  
- 相爱天数按本地日期自动计算  
