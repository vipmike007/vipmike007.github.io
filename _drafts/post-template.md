---
title: Your post title
title_zh: 文章中文标题（可选）
description: One sentence shown on the blog list and in search results.
description_zh: 中文摘要（可选）
tags: [Tag1, Tag2]
---

<!--
Option A: write in ONE language — just delete the two <div> wrappers below and write normally.
          The post shows for both EN and 中文 visitors.
Option B: write in BOTH languages — keep the wrappers. Visitors see the one matching the switch.
          Keep the blank lines right after <div ...> and before </div>, or Markdown won't render.
-->

<div class="en" markdown="1">

Opening paragraph in English.

## A section heading

Normal text, **bold**, *italic*, and a [link](https://www.redhat.com).

- Bullet one
- Bullet two

> A quote or callout.

```bash
oc get pods -n openshift-monitoring
```

</div>

<div class="zh" markdown="1">

中文开头段落。

## 小标题

正文，**加粗**，*斜体*，以及[链接](https://www.redhat.com)。

- 要点一
- 要点二

</div>
