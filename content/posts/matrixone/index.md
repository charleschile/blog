---
draft: false
title: "MatrixOne开源开发经历"
date: '2024-07-24T10:35:26+08:00'
summary: "MatrixOne开源开发经历"
description: "MatrixOne开源开发经历"
toc: true
readTime: true
autonumber: false
math: true
tags: ["database", "golang"]
showTags: true
hideBackToTop: false
---

## 记录
### 7.24
tasks

#### embedding function
- [ ] update the embedding description and document

#### chunk function
we need to support chunk function in such a way that it accepts a URL or a data link. And then it will read from that particular file and then chunk the files. 

But we'll need to support Chunk for detailing as well so as in like, basically, we need to read a file and then, do the chunking on that particular file and then output that particular jump as combination of file URL offset and size.

Instead of that, you should be outputting file URL this thing in size if it is off type.

Loadfile function is being modified!

> LOAD_FILE -> 2 overloads -> return text type
> 
> It was not designed to read files from all the rules or something of that sort. it would just read files from the 1st row
>
> ReadFromFIle function 
>
> 14:45
>
> python api
>
> python api where diffferent chunkings are implemented already
>
> Find out some python libraries and sample codes which are particularly used by this Llm model and all those things to do chunking, and then try to incorporate that paricular strategy in.


- [ ] read a file 
- [ ] do the chunking
