---
layout: 2022
title: about
css: "main{padding:0 1rem 1rem;} h2{text-align:left; margin-bottom:-.95em;} .box{max-width:35rem; padding:.5em .05em;} @media only screen and (min-width:575px){h2{padding-right:8em;}}"

qna:
  - question: "define:ArtFight"
    answer: ArtFight is a month-long art trading competition, in which participants earn points for drawing each others’ characters. More info on [the official about page](https://artfight.net/info/about)!
  - question: Who are you? Why this site?
    answer: |-
      [NightAuctor](https://artfight.net/~NightAuctor) on ArtFight, <a href="/" target="_blank">a-flyleaf</a> elsewhere! Digital artist, here for a good time, posts art almost exclusively to [deviantArt](https://a-flyleaf.deviantart.com/) and/or my own site these days.
      
      I'm a stickler for archival and I don't like that most of the official website is inaccessible to guests, so I made this place to show everything off!
  - question: My art and/or <a href='artists'>links</a> are here; I want them taken down!
    answer: |-
      Sorry about that! Contact me onsite or dA (links above; you’ll get a faster response on dA) and I’ll note that your attack and/or info can only be viewed onsite.
      
      Note: If it's art *I* made, I probably won't take it down---but can remove the recipient info on request.
  - question: social media links broke
    answer: |-
      Everything is up-to-date as of <b>August 3, 2022</b>\*; in the interest of not stalking people, I won’t be updating them---*unless*:
      - the person contacts me to update/remove their links, <em style="font-style:normal;text-transform:uppercase;">or</em>
      - the person shows up again (I draw for them and/or they draw for me) in a future year.
      
      \*Disclaimer: I was originally going to leave 2021 links alone, but updated them in the process of overhauling the site for 2022. The backend has better forward-compatibility now, so this shouldn't happen again <span style="display:inline-block;">>_>\"</span>)
  - question: You drew something for me; what can I do with it?
    answer: |-
      ~Whatever you want~, my dude.
      
      No, seriously. Reupload to character galleries! Use in edits! Print it, trace it, crop it! I do not care. It's yours now, be free.
      
      The **only** caveat is that I want credit for the original work! The names <i>NightAuctor</i> and <i>a-flyleaf</i> both work; I'd *prefer* a non-ArtFight link (either to [my deviantArt](https://www.deviantart.com/a-flyleaf) or this website), but both names should lead back to me regardless.
  - question: Do you have a Toyhouse or other platform?
    answer: |-
      Toyhouse: No, but I made [my own version which is for me](https://a-flyleaf.github.io/toyshelf) ᕕ(&nbsp;ᐛ&nbsp;)ᕗ Everyone I threw on ArtFight can also be found there!
      
      Other platforms: Probably not! (Yes, you can reupload art I made for you on $socialMediaOfYourChoice, ↑with credit↑.) You can find other internet corners I may be lurking around through [my base site](https://a-flyleaf.github.io).
---
{%for faq in page.qna%}<section><h2>{{faq.question}}</h2><div class="box">{{faq.answer|markdownify}}</div></section>{%endfor%}