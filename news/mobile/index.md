---
title: News
---
<style>
h1 {text-align: center;}
h2 {text-align: left;}
h4 {text-align: center;}
h3 {text-align: left;}
p {text-align: center;}
a:link { text-decoration: none;}
a:active { text-decoration: none}
a:hover { text-decoration: none;}
a:visited { text-decoration: none;}
</style>
<style type="text/css">
  #left{
        text-align:left;
  }
  #right{
        text-align:right;
  }
  #title{
        font-size:20px;
        text-align:center;
        font-weight:bold;
  }
  #des{
        font-size:12.5px;
        text-align:left;
  }
  #center{
          text-align: center;
  }
  .block{
         display: inline-block
  }
  .blank{
         display: inline-block;
         width: 20px;
         height: 20px;
  }
  hr{
     margin: 20px auto;
  }
  .banner{
                 font-size:12.5px;
                 line-height: 40px;
                 background-color: #f0f0f0;
                 weight: 100%;
                 color: #000000;
                 text-align: center;
  }
  li{
     list-style-type:none
  }
  ul{
     margin:0;
     padding:0
  }
</style>
<div class="banner">If you're desktop users, please click <a href="news/">here</a>.</div>
<div style="height: 30px"></div>
<h1><div id="left">News</div></h1>
<hr>
<ul>
  {% for post in site.posts %}
    <li>
      <div>
  <a href="{{ post.url }}">
    <div style="width: 100%;">
    <img src="{{ post.rimg }}" style="width: 100%">
      <div class="blank"></div>
    <div style="vertical-align:top;display: inline-block">  
    <div class="block" style="height:20px"><p id="des" style="color:#727272;">{{ post.date | date: "%-d %B %Y" }}</p></div>
    <br>
      <div class="block" style="height:20px;color: black"><p id="title">{{ post.title }}</p></div>
    <br>
      <p style="color:#727272;" id="center">{{ post.des }}</p>
    </div>
    </div>
  </a>
</div>
    </li>
  {% endfor %}
</ul>
