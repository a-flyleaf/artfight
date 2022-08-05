---
layout: 2022
title: art for you
css: main{text-align:center;} main p{max-width:24em;} .ff{background:red;}
---
...and by "you" I mean the attack recipients <span style="display:inline-block;">:V</span>

## 2021: <b class="y2021">Team Cyberpunk</b>
**24** attacks, **7** of which were friendly fires
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.artist=='NightAuctor'%}{%capture year%}{{art.time|date:"%Y"}}{%endcapture%}{%if year == "2021"%}<figure><a href="{%include url.html%}/assets/img/atk/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>for</a> <a href='{%include url.html%}/artists#{{art.for}}' target='_blank'><b>{{art.for}}</b></a></p>"><img src="{%include url.html%}/assets/img/atk/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endif%}{%endfor%}</div>

## 2022: <b class="y2022">Team Bloom</b>
**25** attacks, **8** friendly fires
<div class="gallery five">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.artist=='NightAuctor'%}{%capture year%}{{art.time|date:"%Y"}}{%endcapture%}{%if year == "2022"%}<figure><a href="{%include url.html%}/assets/img/atk/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>for</a> <a href='{%include url.html%}/artists#{{art.for}}' target='_blank'><b>{{art.for}}</b></a></p>"><img src="{%include url.html%}/assets/img/atk/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endif%}{%endfor%}</div>