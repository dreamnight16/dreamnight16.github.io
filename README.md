# 梦夜の小窝awa

> 一个无聊的博客 —— 梦夜十六的个人博客

本站基于 [Hexo](https://hexo.io/) 静态博客框架构建，使用 [NexT.Gemini](https://theme-next.org/) 主题，托管于 GitHub Pages。

- 线上地址：<https://dreamnight16.github.io/>
- 自定义域名：<http://dreamnight.net.cn/>

## 仓库说明

本仓库仅包含 Hexo 生成的**静态站点产物**（即 `hexo generate` 输出的 `public/` 目录内容），不包含 Hexo 源码（`source/`、`_config.yml`、主题配置等）。Hexo 源码维护于独立仓库中，构建后再将 `public/` 目录同步到本仓库。

## 构建与部署

在 Hexo 源码目录中执行：

```bash
# 安装依赖
npm install

# 本地预览
hexo server

# 生成静态文件（输出到 public/）
hexo generate
```

将 `public/` 目录的内容提交到本仓库的 `master` 分支，GitHub Pages 会自动发布：

```bash
# 方式一：使用 hexo-deployer-git 一键部署（需在 _config.yml 中配置 repo）
hexo deploy

# 方式二：手动将 public/ 内容推送至本仓库
cd public && git init && git add -A && git commit -m "Site updated" \
  && git push -f https://github.com/dreamnight16/dreamnight16.github.io.git master
```

## 许可

[MIT](LICENSE)
