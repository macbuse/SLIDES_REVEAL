# Multimedia Slides with reveal.js

I compiled the 
[file](https://macbuse.github.io/SLIDES/myslides.html)
 from the markdown using **pandoc**

- it's quite fast but doesn't appear to give me much control, maybe write
  a python script to do it later
- I had to use html **audio** tags as I needed autoplay behavior that
  **reveal** blocks :(

```pandoc -t revealjs -s -o myslides.html slides.md -V revealjs-url=https://unpkg.com/reveal.js@3.9.2/ -i --mathjax```

-i is important stands for incremental !!

---

## The voice is compiled like this:

well it's what is available client side :(

```flite -t "I have always wondered what it would be like to be Hawkings" -o word2.wav```

```ffmpeg -i word2.wav -acodec mp3 word3.mp3```

actually for my second attempt I used python and **gtts** <br>
WTF it's a-fecking-mazing 
[see here](https://macbuse.github.io/DAO/myslides.html)
but
 
- it is server side
- I don't know how many requests you are limited to on a free tier
