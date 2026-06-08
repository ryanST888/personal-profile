# 个人网站起步指南

这个项目是一个用于求职投递的单页个人网站。第一版先把招聘方最关心的信息放清楚：你是谁、想投什么岗位、做过什么项目、会什么技术、怎么联系你。

## 本地预览

直接双击 `index.html` 可以打开。更推荐在当前文件夹运行：

```powershell
node server.mjs
```

然后访问 `http://127.0.0.1:8080`。

## 第一步：替换基础信息

在 `index.html` 里搜索并替换这些内容：

- `你的姓名`
- `your.email@example.com`
- `https://github.com/yourname`
- `https://www.linkedin.com/in/yourname`
- `Software Engineer · Open to Work`
- 首页第一段自我介绍

语言切换文案集中在 `script.js` 的 `translations` 对象里。需要调整繁体中文、简体中文或英文内容时，优先改那里。

## 第二步：写项目

每个项目建议写成 3 句话：

1. 这个项目解决了什么问题。
2. 你具体负责什么。
3. 最后有什么结果，例如上线、完成演示、提升效率、支持多少用户、获得什么反馈。

## 第三步：写经历

经历不用像简历一样堆满。网站上每段经历保留最强的 1 到 2 个结果即可。招聘方如果感兴趣，会再打开你的简历或项目链接。

## 第四步：换视觉图

当前 `assets/portfolio-visual.png` 是占位图。你可以替换成：

- 个人职业头像
- 项目截图拼图
- 你最想展示的作品界面

如果替换图片，保持文件名不变最省事。

## 第五步：部署

最简单的路线是 GitHub Pages：

1. 把项目推送到 GitHub 仓库。
2. 在仓库 Settings 里打开 Pages。
3. Source 选择 `Deploy from a branch`。
4. Branch 选择 `master` 或 `main`，目录选择 `/root`。

之后你会得到一个可以放进简历的公开网址。
