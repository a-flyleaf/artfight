---
layout: 2022
title: art for me
css: main{text-align:center;} main p{max-width:22em;}
---
<span style="display:inline-block;">&lt;3</span> <span style="display:inline-block;">&lt;3</span> <span style="display:inline-block;">&lt;3</span>

## [2021]({%include url.html%}/art/2021)
**16** defenses!  
Zero and "sawface" got drawn the most, with **5** attacks each! (3 each for the cringetober duo)
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.for=='NightAuctor'%}{%capture year%}{{art.time|date:"%Y"}}{%endcapture%}{%if year == "2021"%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def{%if art.ff%} ff{%endif%}" data-fancybox="2021" data-caption="<p class='tofrom'><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>{%if art.cptn%}<p class='cptn'>{{art.cptn}}</p>{%endif%}"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endif%}{%endfor%}</div>

## [2022]({%include url.html%}/art/2022)
**15** defenses!  
"Sawface" got drawn most, with **7** attacks! (Zero 2, entity 3, toolbelt kid 1, and 2 for "wolf-skull" (new this year))
<div class="gallery five">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.for=='NightAuctor'%}{%capture year%}{{art.time|date:"%Y"}}{%endcapture%}{%if year == "2022"%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def{%if art.ff%} ff{%endif%}" data-fancybox="2022" data-caption="<p class='tofrom'><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a>{%if art.cptn%}<p class='cptn'>{{art.cptn}}</p>{%endif%}"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endif%}{%endfor%}</div>

Character info, references, and galleries are organized [on a subpage here]({%include url.html%}/etc/roster).