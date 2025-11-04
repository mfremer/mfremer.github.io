# mfremer.github.io
Personal website, build locally and pushed to github. Workflow is detailed in [here](https://www.rueth.info/multilingual-github-pages/prerequisites/). For more info about `git worktree` see [here](https://stackoverflow.com/questions/45491328/git-add-a-worktree-from-existing-remote-branch)

## How to setup locally
```bash
# Clone repository
git clone git@github.com:mfremer/mfremer.github.io
git worktree list
git worktree add docs/_site site
cd docs
bundle install
```

## Deploying the site
### Manually
```bash
cd docs
bundle exec jekyll build
cd _site
touch .nojekyll
git add/commit/push
```
### Automatically
ATTENTION: does not work properly, I should fix it sometime...
```bash
cd docs
rm -r _site
cd ..
./deploy.sh
```

## Building/serving site locally
```bash
bundle exec jekyll clean # sometimes avoids errors with remote-theme
bundle exec jekyll build # or
bundle exec jekyll serve
```
