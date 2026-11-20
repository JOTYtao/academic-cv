# Tao Jing · Academic Website

An English-language academic portfolio based on the [HugoBlox Academic CV template](https://github.com/HugoBlox/hugo-theme-academic-cv).

## 维护内容

| 内容 | 文件 |
| --- | --- |
| 个人简介、学术邮箱、教育与任职经历 | `data/authors/me.yaml` |
| 首页与精选论文区块 | `content/_index.md` |
| 首页下载的公开版简历 | `static/uploads/CV_JING_Tao.pdf` |
| 研究方向 | `content/research.md` |
| 教学与学术服务 | `content/experience.md` |
| 论文与 DOI | `content/publications/<slug>/index.md` |
| 导航 | `config/_default/menus.yaml` |

新增论文时，可复制一篇现有论文的目录，更新标题、作者、年份、期刊与 DOI。设置 `featured: true` 后，论文会出现在首页。

## 预览与部署

使用 Hugo Extended 0.162.0、Go、Node.js 22 和 npm。运行 `npm ci` 后使用 `npm run dev` 本地预览，使用 `npm run build` 构建生产站点。

仓库的 Pages 发布源选择 **GitHub Actions**。提交到 `main` 后自动构建并部署。

首页代表作使用论文页面的 `featured: true` 和 `selected_work` 字段。将论文原图放在对应条目目录的 `featured.png`，将对应的原始图 PDF 放在同一目录的 `framework.pdf`，并更新图注与替代文字。首页按 `selected_work_order` 从小到大排列。
