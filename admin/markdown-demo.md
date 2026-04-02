---
title: Markdown 语法与 Fluid 特色示例
date: 2024-03-30 14:00:00
tags: [Markdown, 示例, Fluid]
index_img: https://images.unsplash.com/photo-1499750310107-5fef28a66643?w=800&q=80
banner_img: https://images.unsplash.com/photo-1499750310107-5fef28a66643?w=1200&q=80
---

这是一篇展示 Markdown 基础语法以及 **Fluid 主题** 特色功能的示例文章。

<!-- more -->

## 1. 基础文本操作

你可以方便地使用 **加粗**、*斜体*、~~删除线~~，或者 [这是一个超链接](https://hexo.io)。

> 这是一个引用块：
> “书山有路勤为径，学海无涯苦作舟。”

---

## 2. 代码块示例 (Code Block)

Fluid 主题对代码块支持非常好，会自动识别语言并添加高亮。

### Python 示例
```python
def hello_world():
    print("Hello, sdkly's blog!")

if __name__ == "__main__":
    hello_world()
```

### JavaScript 示例
```javascript
const blog = {
  owner: "sdkly",
  theme: "Fluid",
  status: "Online"
};
console.log(`Welcome to ${blog.owner}'s blog!`);
```

---

## 3. 图片展示 (Images)

### 网络图片
你可以直接粘贴图片的 URL 地址：

![这是一张来自 Unsplash 的精美图片](https://images.unsplash.com/photo-1488590528505-98d2b5aba04b?w=800&q=80)

### 本地图片 (推荐方式)
1. 将图片放入 `source/images/` 文件夹（如果没有这个文件夹请手动创建一个）。
2. 使用以下语法引用：
   `![图片描述](/images/你的图片名.jpg)`

---

## 4. 列表与任务

- [x] 完成博客搭建
- [x] 更换 Fluid 主题
- [ ] 写第一篇正式博文
- [ ] 学习 Markdown 进阶语法

---

## 5. Fluid 特色：便签 (Note)

这是 Fluid 主题自带的精美组件，非常适合写“提示”或“警告”。

::: note info
**提示**：这是一个信息提示框。
:::

::: note warning
**注意**：这是一个警告框，用来提醒读者注意某些事项。
:::

::: note danger
**危险**：这是一个极其重要的警告，例如删除数据的后果。
:::

---

## 6. 数学公式 (LaTeX)

如果你在配置里开启了 Katex，你甚至可以写复杂的公式：
$E = mc^2$

---

祝你在 `sdkly.qzz.io` 写得开心！
