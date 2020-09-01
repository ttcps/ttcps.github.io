---
title: Update Log
---
<style type="text/css">
.text{
  line-height: 35px;
  font-size: 15px;
  color:black;
  text-align: left;
}
hr{
  margin: 20px auto
}
</style>
<h1 style="text-align: left">Update Log</h1>
<hr>
<detail>
<summary>Versions</summary>
<ul>
{% for version in site.data.versions %}
  <li><p class="text"><a href="/update-log/#{{ version.code }}">{{ version.num }}</a></p></li>
</ul>
</detail>
<hr>
<h1 style="text-align: left" id="{{ version.code }}">{{ version.num }}</h1>
<p class="text">{{ version.content }}</p>
{% endif %}
