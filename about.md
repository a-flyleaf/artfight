---
layout: 2022
title: about
css: "main{padding:0 1rem 1rem;} h2{text-align:left; margin-bottom:-.95em;} .box{max-width:35rem; padding:.5em .05em;} @media only screen and (min-width:575px){h2{padding-right:8em;}}"

qna:
  - question: "define:ArtFight"
    answer: ArtFight is a month-long art trading competition, held every July, in which participants are sorted into two teams and earn points for "attacking" (creating art of) each others' characters. More info on [the official about page](https://artfight.net/info/about)!
  - question: Who are you? Why this site?
    answer: |-
      <b>who</b>: [NightAuctor](https://artfight.net/~NightAuctor) on ArtFight, <a href="/" target="_blank">a-flyleaf</a> here! Digital artist, here for a good time. I don't post my art online much these days, but when I do it's probably on my own site somewhere.
      
      <b>why</b>: I'm a stickler for archival, and I don't like that most of the official ArtFight website is inaccessible to guests. This place exists to show everything off!
  - question: My art and/or <a href='artists'>links</a> are here; I want them taken down!
    answer: |-
      Sorry about that! I'll note that your art and/or links can only be viewed on ArtFight; [contact me](/about#contact). (disclaimer: Onsite messages are *unlikely* to be noticed in a timely manner.)
      
      If it's art I made for you, I'd rather not take it down. But I can remove recipient info on request.
  - question: social media links broke
    id: socmed
    answer: |-
      These get updated when I edit the site. In the interest of not stalking people, I don't touch them again---*unless*:
      - the person contacts me to update/remove their links, <em style="font-style:normal;text-transform:uppercase;">or</em>
      - the person shows up again (I draw for them and/or they draw for me) in a future year.
      
      The year shown may not correlate with the year the artist's work was created. I edit this site very sporadically.
  - question: You drew something for me; what can I do with it?
    answer: |-
      ~Whatever you want~, my dude.
      
      No, seriously. Reupload it to character galleries! Use in edits! Print it, trace it, crop it! I do not care. It's yours now, be free.
      
      The **only** caveat is that I want credit for the original work! The names <i>NightAuctor</i> and <i>a-flyleaf</i> both work; I'd *prefer* a non-ArtFight link (either to [my deviantArt](https://www.deviantart.com/a-flyleaf) or this website), but both names should lead back to me regardless.
  - question: Do you have a Toyhouse or other platform?
    answer: |-
      <b>toyhouse</b>: No, but I made [my own version which is for me](https://a-flyleaf.github.io/toyshelf) ᕕ(&nbsp;ᐛ&nbsp;)ᕗ Everyone I threw on ArtFight can also be found there!
      
      <b>other platforms</b>: Probably not! (Yes, you can reupload art I made for you on $socialMediaOfYourChoice, ↑ with credit ↑.) You can find other internet corners I may be lurking around through [my base site](https://a-flyleaf.github.io).
---
{%for faq in page.qna%}<section{%if faq.id%} id="{{faq.id}}"{%endif%}><h2>{{faq.question}}</h2><div class="box">{{faq.answer|markdownify}}</div></section>{%endfor%}