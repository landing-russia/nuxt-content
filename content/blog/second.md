---
title: MDC
---

# {{ $doc.title}}

MDC stands for _**M**ark**D**own **C**omponents_.

## Next steps


```js
const blogPosts = await queryContent("/blog")
  .sort({ date: -1 }) // show latest articles first
  .where({ _partial: false }) // exclude the Partial files
  .find()
```

😸 👨‍🚀

