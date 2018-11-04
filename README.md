# blog

## GitHub blog load

```bash
git clone git@github.com:jbrette/blog.git
git rm -fr themes/mainroad/
git rm -fr themes/hugo-future-imperfect/
git rm -fr public/
git submodule add https://github.com/jpescador/hugo-future-imperfect themes/hugo-future-imperfect
git submodule add https://github.com/vimux/mainroad themes/mainroad
git submodule add -b master git@github.com:jbrette/jbrette.github.io.git public
```

## Test locally

```bash
hugo server --bind="0.0.0.0"
```

Open browser on http://127.0.0.1:1313

## Public to github.io

```bash
./deploy.sh 
```
