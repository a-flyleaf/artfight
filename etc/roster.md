---
layout: 2022
title: character roster
css: "h2{text-align:left; text-align:center; padding:0 0 .25em; font-size:2em;} blockquote p:last-of-type{margin-bottom:0;} .fancybox__caption a{color:#fff !important;} .refs{max-width:35rem; margin:0 auto; padding-left:1em;} .refs ul,.refs li{display:inline; padding-left:.25em;} .refs li::before{content: '•'; padding-right:.5em;} .refs li:first-of-type::before{content:none;} .refs ul{padding-left:0;} .float{margin:2em auto 0; text-align:center;} .float img{border-radius:5px; border:1px solid #c2c2c2;} hr{margin-top:2em;} #note{text-align:center;} @media only screen and (min-width:1000px){.float img{float:left; width: 150px; margin:.5em 20px 0 -170px;} h2{text-align:left; padding-left:1rem;} #toolbelt .float img,#entity .float img{margin-top:-5px;}} @media (prefers-color-scheme:dark){.float img{border-color:#545454;}}"
---
See [Toyshelf](https://a-flyleaf.github.io/toyshelf) for art by yours truly, and more up-to-date info in general! (Not linking character pages directly because, at the time of writing, my organization over there is a biiiit of a mess and extremely subject to change.... <span style="display:inline-block;">>_>\"</span>)

Names link to ArtFight character pages.

<article id="zero">{%for chara in site.data.roster%}{%if chara.nm=="Zero"%}<p class="float"><img src="{%include url.html%}/assets/img/{{chara.prev}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{{chara.af}}">{{chara.nm}}</a></h2>
	<div class="refs"><b>image references:</b> {{chara.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{chara.desc|markdownify}}</blockquote></details>
	<details><summary>additional note(s)</summary><blockquote>{{chara.perm|markdownify}}</blockquote></details>{%endif%}{%endfor%}
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.char contains 'zero'%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endfor%}</div></article>

----

<article id="sawface">{%for chara in site.data.roster%}{%if chara.nm contains "sawface"%}<p class="float"><img src="{%include url.html%}/assets/img/{{chara.prev}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{{chara.af}}">{{chara.nm}}</a></h2>
	<div class="refs"><b>image references:</b> {{chara.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{chara.desc|markdownify}}</blockquote></details>
	<details><summary>permissions</summary><blockquote>{{chara.perm|markdownify}}</blockquote></details>{%endif%}{%endfor%}
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.for=='NightAuctor'%}<!--prevents the Vaukran cameo from causing problems-->{%if art.char contains 'sawface'%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endif%}{%endfor%}</div>
<p id="note">Not shown: makes a small cameo in <a href="{%include url.html%}/for-you#art-29">an attack I drew</a>!</p></article>

----

<article id="toolbelt">{%for chara in site.data.roster%}{%if chara.nm contains "toolbelt"%}<p class="float"><img src="{%include url.html%}/assets/img/{{chara.prev}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{{chara.af}}">{{chara.nm}}</a></h2>
	<div class="refs"><b>image references:</b> {{chara.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{chara.desc|markdownify}}</blockquote></details>
	<details><summary>additional note(s)</summary><blockquote>{{chara.perm|markdownify}}</blockquote></details>{%endif%}{%endfor%}
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.char contains "toolbelt"%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endfor%}</div></article>

----

<article id="entity">{%for chara in site.data.roster%}{%if chara.nm contains "entity"%}<p class="float"><img src="{%include url.html%}/assets/img/{{chara.prev}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{{chara.af}}">{{chara.nm}}</a></h2>
	<div class="refs"><b>image references:</b> {{chara.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{chara.desc|markdownify}}</blockquote></details>
	<details><summary>additional note(s)</summary><blockquote>{{chara.perm|markdownify}}</blockquote></details>{%endif%}{%endfor%}
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.char contains "entity"%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endfor%}</div></article>

----

<article id="wolfskull">{%for chara in site.data.roster%}{%if chara.nm contains "wolf"%}<p class="float"><img src="{%include url.html%}/assets/img/{{chara.prev}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{{chara.af}}">{{chara.nm}}</a></h2>
	<div class="refs"><b>image references:</b> {{chara.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{chara.desc|markdownify}}</blockquote></details>
	<details><summary>additional note(s)</summary><blockquote>{{chara.perm|markdownify}}</blockquote></details>{%endif%}{%endfor%}
<div class="gallery four">{%assign chrono = site.data.art|sort:"time"%}{%for art in chrono%}{%if art.char contains "wolf"%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def" data-fancybox="art" data-caption="<p><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'><b>{{art.artist}}</b></a></p>"><img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt=""/></a></figure>{%endif%}{%endfor%}</div></article>