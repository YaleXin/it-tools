# 部署到 github pages

官方支持部署到 vercel，没有直接支持部署到github pages。github pages 只支持静态页面，对于 vue 项目可以在构建的时候生成静态页面再打包上传到 github pages 空间。

github actions 中启用workflow "deploy-github-pages.yml"就可以在每次推送代码到远程仓库时构建静态页面并推送 github pages 空间。

注意 github pages设置页面“Build and deployment" -> Source 中选择“Github Actions”（不要选Deploy from a branch）