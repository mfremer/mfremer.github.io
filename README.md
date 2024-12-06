# mfremer.github.io
Personal website, build locally and pushed to github. Workflow is detailed in [here](https://www.rueth.info/multilingual-github-pages/prerequisites/).

## How to setup locally
```bash
# Clone repository
git clone git@github.com:mfremer/mfremer.github.io
cd mfremer.github.io/docs
# Clone current site from live branch
git clone -b site --single-branch git@github.com:mfremer/mfremer.github.io _site
bundle install
```

## Deploying the site
```bash
chmod u+x deploy.sh # if necessary
./deploy.sh
```

## Building/serving site locally
```bash
bundle exec jekyll clean # sometimes avoids errors with remote-theme
bundle exec jekyll build # or
bundle exec jekyll serve
```