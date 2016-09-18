---
layout: post
title: "使用Octopress寫部落格"
date: 2016-08-21 02:00:49 +0800
comments: true
categories: [Octopress, blog]
published: false
---

要先安裝git和ruby

``` bash
git clone git://github.com/imathis/octopress.git octopress
cd octopress
bundle install
rake install
```

在github上新建一個repo，命名為 `your_username.github.io` ，your_username請自行替換為你的github帳號的名稱

``` bash
rake setup_github_pages
```

將`https://github.com/Kamigami55/Kamigami55.github.io.git`貼進去

``` bash
rake generate
rake deploy

```

``` bash
git add .
git commit -m 'Start my blog'
git push origin source
```

至此就可以在`https://kamigami55.github.io/`看到你的部落格了！（只有好好看的外觀而已，完全還沒有內容）
