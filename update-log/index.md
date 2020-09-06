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
.atext{
  line-height: 35px;
  font-size: 15px;
  color:black;
  text-align: left;
}
hr{
  margin: 20px auto
}
h1{
  text-align: center
}
</style>
<h1 style="text-align: left">Update Log</h1>
<hr>
<details>
  <summary><span class="text">Versions</span></summary>
{% for version in site.data.versions %}
<ul>
  <li><<a href="/update-log/#{{ version.code }}" class="atext">{{ version.num }}</a></li>
</ul>
{% endfor %}
</details>
{% for version in site.data.versions reversed %}
<hr>
<h1 style="text-align: left" id="{{ version.code }}">{{ version.num }}</h1>
<p class="text">{{ version.content }}</p>
{% endfor %}
