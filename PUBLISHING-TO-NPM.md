# Publishing to npm:

## Manual Way
```bash
   git pull https://github.com/rails/jquery-ujs.git master
   vim package.json # updating version number
   git commit -am 'the version number'
   git push --follow-tags origin master
   npm publish
```

## release-it
Alternately, I use [release-it](https://github.com/webpro/release-it). Assuming the version is 1.2.1 to publish:

```
git pull https://github.com/rails/jquery-ujs.git master
release-it 1.2.1
```

Take the defaults, except answer y to the final question to publish.
