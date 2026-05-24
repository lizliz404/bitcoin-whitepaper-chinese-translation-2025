# 比特币白皮书中文翻译 2025

《Bitcoin: A Peer-to-Peer Electronic Cash System》的中文翻译与在线阅读版本，由 Liz 整理、翻译与校订。

- **在线阅读**：https://bitcoin-whitepaper.lizliz.xyz/
- **Markdown 原文**：[zh.md](zh.md)
- **项目状态**：静态内容项目，已完成，后续仅做错别字、链接、SEO 与展示细节维护

> 致所有信奉“不懂不投”，并愿意回到第一性原理读源头文本的人。

## 项目特色

- **中英对照精读**：保留白皮书原始结构、公式、图示与参考文献，便于逐段理解。
- **中文表达校订**：在参考李笑来 2018 年译本的基础上，结合多轮校对，尽量兼顾准确、顺畅与可读性。
- **低干扰阅读页**：提供独立静态站点，包含目录、脚注、公式渲染、图示展示与移动端适配。
- **SEO 友好**：配置 canonical、robots、sitemap、Open Graph、Twitter Card、JSON-LD 与 favicon / social image assets，方便搜索引擎和社交平台抓取。

## 为什么重新翻译

比特币白皮书不是营销材料，也不是二手解读。它是一份很短、很密、很干净的技术方案：指出双花问题，提出点对点电子现金系统，并说明如何用工作量证明和最长链规则解决共识问题。

重新翻译它的价值不在于“又多一个译本”，而在于把阅读过程变成一次强制精读：每个词、每个公式、每张图都必须重新面对，不能靠熟悉感糊弄过去。

## 文件结构

```text
.
├── index.html          # 在线阅读页
├── zh.md               # 中文翻译正文
├── images/             # 白皮书正文图示
├── assets/             # favicon、PWA icon、OpenGraph 图片等站点资产
├── progress/           # 翻译/页面制作过程中的历史草稿与记录
├── robots.txt          # crawler 指引
├── sitemap.xml         # 搜索引擎 sitemap
├── site.webmanifest    # PWA/浏览器图标声明
└── _headers            # Cloudflare Pages headers
```

## 本地预览

这是纯静态项目，不需要构建步骤。

```bash
python3 -m http.server 8765
```

然后打开：

```text
http://127.0.0.1:8765/
```

也可以直接在浏览器打开 `index.html`，但用本地 HTTP server 更接近线上环境。

## 维护说明

- 正文内容优先改 `zh.md`。
- 阅读页样式和 SEO metadata 在 `index.html`。
- 社交分享图、favicon、PWA icons 放在 `assets/`。
- 如果改了 URL、标题、描述或图片路径，同步检查：`index.html`、`robots.txt`、`sitemap.xml`、`site.webmanifest`、`_headers`。

## 致谢

- Satoshi Nakamoto，原文作者。
- 李笑来老师 2018 年中文译本，为本版本提供重要参考。
- 所有愿意认真读原文、指出翻译问题的人。

## License

原始白皮书版权归原作者所有。本仓库中的中文翻译和页面整理部分暂未指定开源许可证；引用或再发布前请保留来源说明。
