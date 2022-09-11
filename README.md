## Minify JS scripts (order is important)
```
uglifyjs jquery.js bootstrap.min.js vegas.min.js modernizr.custom.js toucheffects.js  owl.carousel.min.js smoothscroll.js wow.min.js custom.js lightbox.js > script.min.js 
```

## Production - dockerize website

Build docker image:

```bash
docker build -t mathildevedel .
```

Run docker image:
```bash
docker run --name mathildevedel-container -p 80:80 mathildevedel
```