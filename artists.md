---
layout: 2022
title: artist directory
css: "
	main{padding:0 1rem 1rem;}
	
	.nm{max-width:35rem; margin:0 auto -1.25em; padding:.25rem 0 0 .5rem;}
	h2{text-align:left; display:inline-block; padding:1rem .5rem 0;}
	h2 a{text-decoration:none;}
	small{display:inline-block; padding-left:.5rem; opacity:.5;}
	
	.box{max-width:35rem; padding:1em .05em;} .box p{margin:0;} 
	
	small{font-size:.85em;}
"
---
Links were recorded in the noted year, and copied as they appear onsite (including custom site titles). They are *not* kept up-to-date; see [the about page]({%include url.html%}/about#socmed) for details.

----

{%assign rtst = site.data.artists|sort_natural:"un"%}{%for artist in rtst%}<article id="{{artist.un}}"><div class="nm"><h2><a href="https://artfight.net/~{{artist.un}}">{{artist.un}}</a></h2><small>({{artist.dt}})</small></div>
<div class="box">{%if artist.nolinks%}<p><i>[no links given]</i></p>{%else%}<ul>
	{%if artist.da%}<li>deviantArt: <a href="https://{{artist.da}}.deviantart.com/">{{artist.da}}</a></li>{%endif%}
	{%if artist.fa%}<li>FurAffinity: <a href="https://www.furaffinity.net/user/{{artist.fa}}">{{artist.fa}}</a></li>{%endif%}
	{%if artist.ws%}<li>Weasyl: <a href="https://www.weasyl.com/~{{artist.ws}}">{{artist.ws}}</a></li>{%endif%}
	{%if artist.tb%}<li>tumblr: <a href="https://{{artist.tb}}.tumblr.com/">{{artist.tb}}</a></li>{%endif%}
	{%if artist.tw%}<li>Twitter: <a href="https://twitter.com/{{artist.tw}}">{{artist.tw}}</a></li>{%endif%}
	{%if artist.ig%}<li>Instagram: <a href="https://instagram.com/{{artist.ig}}">{{artist.ig}}</a></li>{%endif%}
	{%if artist.th%}<li>Toyhouse: <a href="https://toyhou.se/{{artist.th}}">{{artist.th}}</a></li>{%endif%}
	{%if artist.sh%}<li>Sheezy: <a href="https://sheezy.art/{{artist.sh}}">{{artist.sh}}</a></li>{%endif%}
	{%if artist.bs%}<li>Bluesky: <a href="https://bsky.app/profile/{{artist.bs}}">{{artist.bs}}</a></li>{%endif%}
	{%if artist.uv%}<li>Unvale: <a href="https://unvale.io/{{artist.uv}}">{{artist.uv}}</a></li>{%endif%}
	{%if artist.cr%}<li>Cara: <a href="https://cara.app/{{artist.cr}}">{{artist.cr}}</a></li>{%endif%}
	{%if artist.site-url%}<li>Custom Site: {%if artist.un != "NightAuctor"%}“{%endif%}<a href="{{artist.site-url}}">{%if artist.site-nm%}{{artist.site-nm}}{%else%}{{artist.site-url}}{%endif%}</a>{%if artist.un != "NightAuctor"%}”{%endif%}</li>{%endif%}
</ul>{%endif%}</div></article>{%endfor%}