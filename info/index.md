---
title: Information / 网站资讯
version: Insider Beta (Preview)
version-num: 0.90
---

<style>
h1 {text-align: center;}
h4 {text-align: center;}
h3 {text-align: center;}
p {text-align: center;}
</style>
<style type="text/css">
  #left{
        text-align:left;
  }
  #right{
        text-align:right;
  }
  #center{
        text-align:center;
  }
  .banner{
                 font-size:12.5px;
                 line-height: 40px;
                 background-color: #f0f0f0;
                 weight: 100%;
                 color: #000000;
                 text-align: center;
  }
  #text{
        line-height: 35px;
        font-size: 15px;
        color:black;
        text-align: left;
</style>
{% if page.version ==  "Insider Beta (Preview)" %}
  {% assign version-ch = "內部测试（预览）" %}
{% endif %}


<p id="text">Website version: {{ page.version }}, {{ page.version-num }}-{{ site.github.build_revision | truncate: 6, "" }}<br>Copyright © 2020 tcps/Information Department all right reserved.<br>Powered by GitHub Pages<br>Written by html<br>
<h1 id="left">Copyright Info</h1>
<p id="text">Bigday, bignews.(Aritcle of 1st anniversary) image 1, credit to Maximum(Yeyuxing)</p>
<hr>
<p>Due to the large amount of content, we can't record all, if copyright infringes, please contact us.</p>
<hr>
<p id="text">----------</p>
<p id="text">网站版本：{{ page.version-ch }}，{{ page.version-num }}-{{ site.github.build_revision | truncate: 6, "" }}
<br>
  Copyright © 2020 tcps/资讯部 保留所有权利。<br>由 GitHub Pages 提供技术支持<br>使用html编写<br></p>
<h1 id="left">版权资讯</h1>
<p id="text">Bigday, bignews.(一周年纪念文章) 图一, 由夜雨行（Maximum）授权提供</p>
<hr>
<p>因内容众多，未能尽录，如侵犯版权，请版权方与我们联络。</p>
