---
layout: 2022
title: all the art. All Of It
css: main{text-align:center;} .atk{border-style:dotted !important;}
---
Congratulations, you won!

caption links open in new tabs  
"for"/"from" = attack on ArtFight,  
usernames = artist's social media

<div class="gallery five">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}<figure><a href="{%include url.html%}/assets/img/{%if art.artist == 'NightAuctor'%}atk/{%else%}def/{%endif%}{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}}{%if art.artist=='NightAuctor'%}{%else%} def{%endif%}{%if art.ff%} ff{%endif%}" data-fancybox="art" data-caption="<p>{%if art.artist=='NightAuctor'%}<a href='https://artfight.net/attack/{{art.link}}' target='_blank'>for</a> <a href='{%include url.html%}/artists#{{art.for}}' target='_blank'><b>{{art.for}}</b></a>{%else%}<a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a>{%endif%}</p>"><img src="{%include url.html%}/assets/img/{%if art.artist == 'NightAuctor'%}atk/{%else%}def/{%endif%}{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endfor%}</div>