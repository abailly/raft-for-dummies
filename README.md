To build:

Download [reveal.js](https://github.com/hakimel/reveal.js):

> wget https://github.com/hakimel/reveal.js/archive/master.zip

Use [pandoc](http://johnmacfarlane.net/pandoc/) to generate slides. `h1` tags are replaced with `h3` as their size is too large in
 default style:

>  pandoc --slide-level 1 --variable theme=beige -i -s -o slides.html -t revealjs slides.md && sed -i -e s/h1/h3/g slides.html
