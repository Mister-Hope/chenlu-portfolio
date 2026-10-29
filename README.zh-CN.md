# 陈璐 · 个人简历

> [🇬🇧 English](./README.md)

**陈璐**的个人简历与作品集网站。东北师范大学凝聚态物理专业博士研究生，正在求职**高中物理教师**岗位。

站点为双语结构：英文位于 `/`，中文位于 `/zh/`。

## 关于

- 东北师范大学物理学本硕博贯通培养，推免保送。
- 四年高中物理教学与教研实践，熟悉高中物理知识体系与高考考查重点。
- 连续六年学生工作经历：本科年级长、研究生年级负责人、学生会秘书长。
- 以第一作者身份在 _Light: Science & Applications_、_Physical Review Research_、_J. Mater. Chem. C_ 等期刊发表论文。

## 站点板块

| 板块           | 内容                             |
| -------------- | -------------------------------- |
| 个人资料       | 基本信息、证书与联系方式         |
| 求职意向       | 以教学为核心的求职目标与联系方式 |
| 教育背景与经历 | 学历、教学经历、支教与科研项目   |
| 代表性科研成果 | 第一作者与共同一作论文及期刊分区 |
| 学术合作       | 合作署名论文                     |
| 荣誉与奖项     | 奖学金、荣誉称号与竞赛获奖       |
| 学生工作       | 担任的学生干部职务与职责         |
| 自我评价       | 个人优势与从教意愿总结           |

## 本地开发

```bash
pnpm ci          # 安装依赖
pnpm run dev     # 启动开发服务器 http://localhost:3000
pnpm run build   # 类型检查并构建到 dist/
pnpm run preview # 预览生产构建
pnpm run lint    # 代码检查与格式化
```

## 内容维护

所有面向用户的内容都集中在 [`config.yml`](./config.yml) 中，按语言区分（`/` 为英文，`/zh/` 为中文）。修改内容无需改动源码。

- 文案、链接、板块、媒体 → `config.yml`
- 样式微调 → 项目根目录的 `custom.css`（构建时自动注入）
- 完整配置说明 → [`docs/en.md`](./docs/en.md) / [`docs/zh.md`](./docs/zh.md)

## 部署

推送到 `main` 分支会触发 `Deploy Docs` GitHub Actions 工作流，自动构建并将 `dist/` 发布到 `gh-pages` 分支，通过 GitHub Pages 提供服务。同一份 `dist/` 产物也可部署到 Vercel、Netlify 或任意静态服务器。

## 技术栈

- React 19 + Vite 8，TypeScript
- Tailwind CSS v4
- Iconify 图标
- 使用 markdown-it 渲染 Markdown，并通过自定义 Vite 插件实现静态站点生成

## 项目结构

```text
.
├── config.yml          # 全站内容（英文 + 中文）
├── custom.css          # 自定义样式覆盖，自动注入
├── public/             # 静态资源（头像、背景图）
├── src/                # React 组件与样式
├── lib/                # 配置加载、Markdown 渲染、SSG 插件
├── docs/               # 配置参考文档
└── examples/           # 其他格式的示例配置
```

## 联系方式

- 邮箱：[chenl987@nenu.edu.cn](mailto:chenl987@nenu.edu.cn)
- ORCID：[0009-0006-5397-4679](https://orcid.org/0009-0006-5397-4679)
- 简历：<https://chenlu-resume.innenu.com>
