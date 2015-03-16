# Simple Docker Container for Jekyll Work

Docker Hub: <https://registry.hub.docker.com/u/danshan/docker-jekyll/>

Use example:

```
sudo docker run --rm -v "$PWD:/src" danshan/docker-jekyll build
```

or for repeated calls:

```
alias jekyll='sudo docker run --rm -v "$PWD:/src" -p 4000:4000 danshan/docker-jekyll'
jekyll build
jekyll serve -H 0.0.0.0
```

run as a background daemon:
```
sudo docker run -d -v "$PWD:/src" -p 4000:4000 danshan/docker-jekyll serve -H 0.0.0.0
```

## Goodies
 - Supports pygments syntax highlighting
 - Supports Github Pages
 - Supports Jekyll Redirect From
 - Supports Kramdown
 - Supports RDiscount
 - Supports Rouge


# License: Public Domain

Do what you want!
