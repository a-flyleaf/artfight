---
layout: 2022
title: artist directory
css: main{padding:0 1rem 1rem;} h2{text-align:left; margin-bottom:-.95em; padding-top:.25rem;} h2 a{text-decoration:none;} .box{max-width:35rem; padding:1em .05em;} .box p{margin:0;} small{font-size:.85em;} @media only screen and (min-width:575px){h2{padding-right:8em;}}
---
Links are up-to-date as of **August 3, 2022**, copied as they appear onsite (including custom site titles), and **will not be updated**; see [the about page]({%include url.html%}/about) for details.

----

{%assign rtst = site.data.artists|sort_natural:"un"%}{%for artist in rtst%}<article id="{{artist.un}}"><h2><a href="https://artfight.net/~{{artist.un}}">{{artist.un}}</a></h2><div class="box">{%if artist.nolinks%}<p>[no links given]</p>{%else%}<ul>
	{%if artist.da%}<li>deviantArt: <a href="https://{{artist.da}}.deviantart.com/">{{artist.da}}</a></li>{%endif%}
	{%if artist.fa%}<li>FurAffinity: <a href="https://www.furaffinity.net/user/{{artist.fa}}">{{artist.fa}}</a></li>{%endif%}
	{%if artist.ws%}<li>Weasyl: <a href="https://www.weasyl.com/~{{artist.ws}}">{{artist.ws}}</a></li>{%endif%}
	{%if artist.tb%}<li>tumblr: <a href="https://{{artist.tb}}.tumblr.com/">{{artist.tb}}</a></li>{%endif%}
	{%if artist.tw%}<li>Twitter: <a href="https://twitter.com/{{artist.tw}}">{{artist.tw}}</a></li>{%endif%}
	{%if artist.ig%}<li>Instagram: <a href="https://instagram.com/{{artist.ig}}">{{artist.ig}}</a></li>{%endif%}
	{%if artist.th%}<li>Toyhouse: <a href="https://toyhou.se/{{artist.th}}">{{artist.th}}</a></li>{%endif%}
	{%if artist.site-url%}<li>Custom Site: {%if artist.un != "NightAuctor"%}“{%endif%}<a href="{{artist.site-url}}">{{artist.site-nm}}</a>{%if artist.un != "NightAuctor"%}”{%endif%}</li>{%endif%}
</ul>{%endif%}</div></article>{%endfor%}

<small>Yes, I know this page is a bit unwieldy. I'll, uh, figure out how to put artist links *with* the attacks next round, maybe....</small> 