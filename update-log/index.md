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
{% for version in site.data.versions %}
<details>
<summary>Versions</summary>
<ul>
  <li><p class="text"><a href="/update-log/#{{ version.code }}">{{ version.num }}</a></p></li>
</ul>
</details>
<hr>
<h1 style="text-align: left" id="{{ version.code }}">{{ version.num }}</h1>
<p class="text">{{ version.content }}</p>
{% endif %}
