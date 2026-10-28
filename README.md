# 徐馨柔的海岛个人网站

这是已构建好的静态网站，可直接上传至 GitHub Pages，无需安装 Node.js 或运行构建命令。

包含最新的个人介绍、六张生活照片、学习经历、联系邮箱，以及电脑端三维海岛、船舶与动态波纹。

## 上传与发布

1. 解压 `github-pages.zip`。不要把 ZIP 文件本身上传来代替网页。
2. 在 GitHub 创建一个新的 **Public（公开）** 仓库，名称可用 `island-portfolio`。
3. 打开仓库的上传文件入口，将解压后文件夹**里面的内容**全部上传，包括 `index.html`、整个 `assets` 文件夹、`.nojekyll` 和此说明文件。保持目录结构，不要额外嵌套一层文件夹。
4. 点击 **Commit changes** 保存到 `main` 分支。
5. 打开仓库 **Settings → Pages**。
6. 在 **Build and deployment** 中，将 **Source** 设为 **Deploy from a branch**。
7. 将 **Branch** 设为 **main**，文件夹选 **/ (root)**，点击 **Save**。
8. 等待发布完成，访问 Pages 页面显示的网站地址。通常为 `https://你的用户名.github.io/island-portfolio/`。

如果上传时没有选中 `.nojekyll`，可以通过 Add file → Create new file 创建同名空文件。

## 仓库文件应当长这样

```text
index.html
.nojekyll
README.md
assets/
  ...网页脚本、样式和六张照片
```

`index.html` 必须直接位于发布分支的根目录。不要只上传 HTML，也不要删除或改名 assets 内的文件。

## 注意

- 本包是电脑端网页，已包含运行需要的三维库和图片，资源路径支持仓库子路径。
- 网站通过 HTTP/HTTPS 访问；本地双击 HTML 不能可靠运行三维模块。
- Google Fonts 无法加载时会使用设备字体。
- 公开发布后，网站中的个人资料、照片与联系邮箱可被访客看到。
- 本包不包含原始简历、手机号码、出生日期、在留资料、开发依赖或旧版网页。
- 日后修改请在原项目源码中更新，再重新构建。此包中的文件是发布产物。

GitHub 官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
