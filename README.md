# Diavolo-KingCrimson.github.io

个人主页，基于 [al-folio](https://github.com/alshedivat/al-folio) v1.x（Jekyll）。

线上地址：<https://diavolo-kingcrimson.github.io>

## 本地预览

需要 Docker（本机已装）。在仓库根目录：

```powershell
docker compose up -d
# 打开 http://localhost:8080/
docker compose down
```

首次启动会构建镜像，需要几分钟；之后是秒级。

## 常改的文件

| 想改什么 | 改哪里 |
| --- | --- |
| 首页简介 | `_pages/about.md` |
| 站点标题、描述、语言 | `_config.yml` 顶部 `title` / `description` / `lang` |
| 邮箱、GitHub、社交链接 | `_data/socials.yml` |
| 头像 | 放 `assets/img/prof_pic.jpg`，再按 `_pages/about.md` 里的注释启用 |
| 新闻 / 项目 / 博客 | `_news/` `_projects/` `_posts/` |
| 出版物 | `_bibliography/papers.bib` |

## 部署

推送到 `main` 分支后，GitHub Actions（`.github/workflows/deploy.yml`）自动构建并发布到 `gh-pages`。
首次部署需要到仓库 Settings → Pages 把 Source 设成 `gh-pages` 分支。

## 注意

- 这是**用户主页**仓库，仓库名必须是 `Diavolo-KingCrimson.github.io`，`_config.yml` 里 `baseurl` 必须为空，否则样式和链接会全挂。
- 模板自带的演示内容（`_posts/` 下的示例文章、`_projects/` 示例、Einstein 头像等）还在，删掉即可。
