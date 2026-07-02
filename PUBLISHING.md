# Publishing Guide

推荐仓库名:

```text
kindergarten-math-quiz
```

推荐仓库地址:

```text
https://github.com/dounaoo/kindergarten-math-quiz
```

## GitHub 发布步骤

1. 打开 GitHub 新建仓库页面:

   ```text
   https://github.com/new
   ```

2. 填写:

   ```text
   Repository name: kindergarten-math-quiz
   Description: 小班数学选择题 Beta，带中文女声语音播报的静态网页练习工具
   Visibility: Public
   ```

3. 不要勾选 `Add a README file`、`.gitignore` 或 `license`，这些文件本地已经准备好了。

4. 创建仓库后，在本目录执行:

   ```bash
   git remote set-url origin https://github.com/dounaoo/kindergarten-math-quiz.git
   git push -u origin main
   ```

## GitHub Pages

如果想用 GitHub Pages 发布:

1. 进入仓库 `Settings`。
2. 打开 `Pages`。
3. Source 选择 `Deploy from a branch`。
4. Branch 选择 `main`，目录选择 `/root`。

## Netlify

如果想用 Netlify 发布，有两种方式:

- 直接把本项目目录拖到 Netlify Drop。
- 在 Netlify 里导入这个 GitHub 仓库，发布目录保持根目录即可。
