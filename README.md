# Portfolio 2

This is my portfolio generator.

## Run locally

First install [Jekyll](https://jekyllrb.com/docs/installation/)

Then install the stuff from the Gemfile.

```powershell
bundle install
```

Then run this site. 

```powershell
bundle exec jekyll serve --config "_config.yml,_local_config.yml"
```

## Run as website via docker

```powershell
docker run -it -p 4000:4000 -e "JEKYLL_ENV=docker"--volume="${PWD}:/srv/jekyll" jekyll/jekyll:latest jekyll serve --config /srv/jekyll/_local_config.yml
```