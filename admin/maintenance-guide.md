# 🚀 sdkly 的博客维护手册

这份文档记录了你管理和维护基于 Hexo + Fluid + Cloudflare Pages 博客的所有核心操作。

---

## 📅 1. 发布新文章 (New Post)

每当你想要写新内容时，请执行以下步骤：

1.  **生成文章文件**：
    在 `my-blog` 根目录下运行：
    ```powershell
    npx hexo new post "文章标题"
    ```
2.  **编写内容**：
    打开 `source/_posts/文章标题.md` 进行编辑。
    *   使用 Markdown 语法编写。
    *   文章顶部的 `---` 之间是配置信息（标题、日期、标签）。
3.  **推送上线**：
    执行 [Git 三部曲](#-3-git-发布三部曲)。

---

## 🛠️ 2. 修改网站配置 (Settings)

如果你想修改网站名称、作者、副标题或语言：

1.  **编辑配置文件**：
    打开根目录下的 `_config.yml`。
2.  **关键字段说明**：
    *   `title`: 网站标题
    *   `subtitle`: 副标题/座右铭
    *   `author`: 你的名字
    *   `language`: `zh-CN` (中文)
3.  **保存并推送**：
    执行 [Git 三部曲](#-3-git-发布三部曲)。

---

## ⬆️ 3. Git 发布三部曲 (Deploy)

这是将你本地的所有修改（写文章、改配置、换主题）同步到互联网的**唯一标准动作**：

1.  **暂存修改**：
    ```powershell
    git add .
    ```
2.  **提交版本记录**：
    ```powershell
    git commit -m "这里写你做了什么，比如：新增关于我页面"
    ```
3.  **推送到 GitHub**：
    ```powershell
    git push
    ```
    *Cloudflare Pages 会在检测到推送后的 1-2 分钟内自动完成构建并更新你的网站。*

---

## 📂 4. 管理旧文章 (Manage Posts)

*   **修改旧文章**：直接找到 `source/_posts/` 下对应的 `.md` 文件，修改内容并保存，然后执行 [Git 三部曲](#-3-git-发布三部曲)。
*   **删除文章**：直接删除 `source/_posts/` 下对应的 `.md` 文件，然后执行 [Git 三部曲](#-3-git-发布三部曲)。

---

## 🎨 5. 自定义 Fluid 主题 (Theme Config)

Fluid 主题的深度自定义（如更换背景图、开启搜索、打赏等）在以下文件中：
*   文件路径：`node_modules/hexo-theme-fluid/_config.yml` (或者你根目录下的 `_config.fluid.yml`)。

---

## 🔍 6. 本地预览 (Preview)

在正式推送到网上前，你可以在本地先预览效果：
1.  运行命令：
    ```powershell
    npx hexo server
    ```
2.  在浏览器访问：`http://localhost:4000`。
3.  按 `Ctrl+C` 停止预览。

---

祝写作愉快！如有任何问题，随时找我。
