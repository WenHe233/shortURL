# 短网址 — Zero-Width Short URL

用不可见的零宽空格（U+200B, U+200C, U+200D, U+FEFF）编码长链接的纯前端短网址工具。

## 使用

```
# API 模式
index.html?url=https://example.com/very-long-url

# 解码跳转
index.html#​‌‍﻿…
```

## 技术

- 编码：URL → UTF-8 字节 → Base-4 零宽字符
- 路由：hash 片段承载编码数据，纯前端无需服务端
- QR：前端 Canvas 生成 / API 兜底
- 单文件，零依赖

## 部署

丢到任意静态托管（Cloudflare Pages / Vercel / GitHub Pages）即可。
