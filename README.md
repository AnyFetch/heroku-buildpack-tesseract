heroku-buildpack-tesseract
===========================


This buildpack is now useless.
You can use https://github.com/ddollar/heroku-buildpack-apt
with
```
echo tesseract-ocr > Aptfile
```


Added the libraries to use Tesseract 3.02.02 on Heroku

This buildpack is built to be used through [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi).
In your app you need to:
```
heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi
```

Then, create a `.buildpacks` file inside your app:
```
https://github.com/heroku/_YOUR_MAIN_BUILDPACK
https://github.com/Papiel/heroku-buildpack-tesseract
```
See the documentation of heroku-build-multi for a detailed explanation
how to use it.

## License
MIT License. Copyright 2013 Marco Azimonti.
