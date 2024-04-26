---
layout:     post
title:      (文章标题)
subtitle:   (副标题)
date:       2024-4-26
author:     (作者名)
header-img: img/the-first.png
catalog:   true
tags:
    - 往事如烟
---
# 一级标题
## 二级标题
（正文内容）



<!-- Gitalk 评论 start  -->
{% if site.gitalk.enable %}
<!-- Link Gitalk 的支持文件  -->
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://unpkg.com/gitalk@latest/dist/gitalk.min.js"></script>

<div id="gitalk-container"></div>
    <script type="text/javascript">
    var gitalk = new Gitalk({
    // gitalk的主要参数
        clientID: `{2995cc9e8a8941cd62c2}`,
        clientSecret: `{33036a899b9b0bd9237428e166147a12cb3f7802}`,
        repo: `{bppec.github.io}`,
        owner: '{bppec}',
        admin: ['{bppec}'],
        id: 'Testpage',
    });
    gitalk.render('gitalk-container');
</script>
{% endif %}
<!-- Gitalk end -->

 <!-- disqus 评论框 start  -->
{% if site.disqus.enable %}

<div class="comment">
    <div id="disqus_thread" class="disqus-thread">
    </div>
</div>
<!-- disqus 评论框 end -->

<!-- disqus 公共JS代码 start (一个网页只需插入一次) -->
<script type="text/javascript">
    /* * * CONFIGURATION VARIABLES * * */
    var disqus_shortname = "{{site.disqus.username}}";
    var disqus_identifier = "{{site.disqus.username}}/{{page.url}}";
    var disqus_url = "{{site.url}}{{page.url}}";

    (function() {
        var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
        dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
        (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
    })();
</script>
<!-- disqus 公共JS代码 end -->
{% endif %}
