---
draft: false
title: "Build Personal Website with Hugo"
date: '2024-07-22T16:41:17+08:00'
summary: "Experience with building and deploying Hugo website"
description: "Experience with building and deploying Hugo website"
toc: true
readTime: true
autonumber: true
math: true
tags: ["database", "java"]
showTags: false
hideBackToTop: false
---
## File
### Front Matter
The front matter at the top of each content file is metadata that describes the content, augments the content, establishes the relationships with other content, controls the published structure of your site, determines template selection.

I choose to use yaml format to define the front matter. It is defined in archetypes/default.md:

```yaml
---
draft: true
title: "Log-Structured Merge Tree"
date: '{{ .Date }}'
summary: "An LSM Tree overview and Java implementation."
description: "An LSM Tree overview and Java implementation."
toc: true
readTime: true
autonumber: true
math: true
tags: ["database", "java"]
showTags: false
hideBackToTop: false
---
```
