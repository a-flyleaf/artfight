---
layout: none
---
Links are up-to-date as of **August 3, 2022**, copied as they appear onsite (including custom site titles). In the interest of not stalking people, these **will not be updated** unless someone EITHER returns in a future round OR requests otherwise by contacting me.

{%assign rtst = site.data.artists|sort_natural:"un"%}{%for artist in rtst%}<ul id="{{artist.un}}">
	<li>ArtFight: <a href="https://artfight.net/~{{artist.un}}">{{artist.un}}</a></li>
	{%if artist.da%}<li>deviantArt: <a href="https://{{artist.da}}.deviantart.com/">{{artist.da}}</a></li>{%endif%}
	{%if artist.fa%}<li>FurAffinity: <a href="https://www.furaffinity.net/user/{{artist.fa}}">{{artist.fa}}</a></li>{%endif%}
	{%if artist.ws%}<li>Weasyl: <a href="https://www.weasyl.com/~{{artist.ws}}">{{artist.ws}}</a></li>{%endif%}
	{%if artist.tb%}<li>tumblr: <a href="https://{{artist.tb}}.tumblr.com/">{{artist.tb}}</a></li>{%endif%}
	{%if artist.tw%}<li>Twitter: <a href="https://twitter.com/{{artist.tw}}">{{artist.tw}}</a></li>{%endif%}
	{%if artist.ig%}<li>Instagram: <a href="https://instagram.com/{{artist.ig}}">{{artist.ig}}</a></li>{%endif%}
	{%if artist.th%}<li>Toyhouse: <a href="https://toyhou.se/{{artist.th}}">{{artist.th}}</a></li>{%endif%}
	{%if artist.site-url%}<li>Custom Site: <a href="{{artist.site-url}}">{{artist.site-nm}}</a></li>{%endif%}
</ul>{%endfor%}