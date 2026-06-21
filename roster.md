---
layout: 2022
title: character roster
css: "
	main>p{text-align:center;}
	
	article{margin:3em 0;}
	h2{text-align:left; text-align:center; padding:0 0 .25em; font-size:2em;}
	blockquote p:last-of-type{margin-bottom:0;}
	.fancybox__caption a{color:#fff !important;}
	
	.refs{max-width:35rem; margin:0 auto; padding-left:1em;}
	.refs ul,.refs li{display:inline; padding-left:.25em;} .refs li{display:inline-block;}
	.refs li::before{content: '•'; padding-right:.5em;}
	.refs li:first-of-type::before{content:none;}
	.refs ul{padding-left:0;}
	
	.float{margin:2em auto 0; text-align:center;}
	.float img{border-radius:5px; border:1px solid #c2c2c2;}
	
	hr{margin-top:2em;}
	#note{text-align:center;}
	@media only screen and (min-width:1000px){
		.float img{float:left; width: 150px; margin:.5em 20px 0 -170px;}
		h2{text-align:left; padding-left:1rem;}
		/*spacing fix*/ .fix .float img{margin-top:-5px;}
	}
	@media (prefers-color-scheme:dark){.float img{border-color:#545454;}}
"
---
Names link to ArtFight character pages.

**Zero**, "**sawface**", and the **Flight Rising catch-all** are long-term mainstays. The others are **cycled out** after a round, but art of them is still welcome! I'm just less attached to them &

{%assign chrono=site.data.art|sort:"time"%}{%for ch in site.data.roster%}<article id="{{ch.id}}"{%if ch.fix%} class="fix"{%endif%}><p class="float"><img src="{%include url.html%}/assets/img/roster/{{ch.id}}.png" alt=""></p>
	<h2><a href="https://artfight.net/character/{%if ch.af%}{{ch.af}}{%else%}1415042.previous-characters{%endif%}">{{ch.nm}}</a></h2>
	<div class="refs"><b>references</b>: {{ch.img|markdownify}}</div>
	<details><summary>info</summary><blockquote>{{ch.desc|markdownify}}</blockquote></details>
	<details><summary>additional note(s)</summary><blockquote>{{ch.perm|markdownify}}</blockquote></details>
	
	<div class="gallery four">{%for art in chrono%}{%if art.char contains ch.id%}<figure><a href="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}.{%if art.file%}{{art.file}}{%else%}png{%endif%}" class="y{{art.time|date:'%Y'}} def{%if art.ff%} ff{%endif%}" data-fancybox="{{ch.id}}" data-caption="<p class='tofrom'><a href='https://artfight.net/attack/{{art.link}}' target='_blank'>from</a> <a href='{%include url.html%}/artists#{{art.artist}}' target='_blank'>{{art.artist}}</a></p>{%if art.cptn%}<p class='cptn'>{{art.cptn}}</p>{%endif%}">
		<img src="{%include url.html%}/assets/img/def/{{art.time|date:'%Y'}}/{{art.img}}x.{%if art.tn%}{{art.tn}}{%else%}png{%endif%}" alt="">
	</a></figure>{%endif%}{%endfor%}</div>
</article>{%endfor%}