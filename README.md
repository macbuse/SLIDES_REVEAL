# This is a test


I compiled the file from the markdown 


pandoc -t revealjs -s -o myslides.html slides.md -V revealjs-url=https://unpkg.com/reveal.js@3.9.2/ -i --mathjax:

-i is important stands for incremental !!

---

## The voice is compiled like this:

flite -t "I have always wondered what it would be like to be Hawkings" -o
word2.wav

ffmpeg -i word2.wav -acodec mp3 word3.mp3
