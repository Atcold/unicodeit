# Python Release

```sh
# python checks
pytest
pylint unicodeit

# create package and upload
python setup.py sdist
twine upload dist/unicodeit...
```


# NPM Release

```sh
# update typescript data
python -m unicodeit.export_data

# typescript checks
npm run lint
npm run test

# rebuild typescript bundles
npm run build

# publish
npm publish
```


# Website update

```sh
# follow steps of NPM release first

# push web folder to gh-pages branch
ghp-import web --no-jekyll --push gh-pages
```
