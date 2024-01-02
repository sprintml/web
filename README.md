# SprintML Website

This is the academic website of the SprintML lab at CISPA.

## About the Website

The template for the website was forked and adapted from
the [Allan Lab](https://github.com/mpa139/allanlab/tree/gh-pages).
The underlying frameworks are Jekyll and some Bootstrap, Bootwatch.

## Acknowledgements

Finally, we would like to acknowledge other academic pages that inspired the design of our website:

- We were inspired by the design of the "Team" page by
  the [Kwiat Lab](https://github.com/KwiatLab/group-website-jekyll?ref=jekyll-themes.com) and integrated their for loop
  in our code to iterate over and display our lab members.
- We took the code to display the calendar icon next to the publication data of blogposts on the overview pages
  from [academicpages](https://github.com/academicpages/academicpages.github.io). The icon itself stems from
  the [Font-Awesome](https://github.com/FortAwesome/Font-Awesome) package.

Please reach out to [Adam Dziedzic](https://adam-dziedzic.com/) and [Franziska Boenisch](https://franziska-boenisch.de/)
for comments or concerns.

## Edits

Deploy the website:
```shell
bash deploy.sh
```

Build and serve the site locally:
```shell
bundle exec jekyll serve --host localhost --port 4000 --incremental --livereload --destination docs
```

Build the site for deployment:
```shell
jekyll build --destination docs
```

Ultimate command, never fails and rebuilds everything from scratch:

```shell
bundle exec jekyll serve --force_polling --livereload --trace --destination docs --incremental
```

On Windows:

```shell
bundle exec jekyll serve --force_polling --livereload --incremental --destination docs
```

Do Live reload:

```shell
bundle exec jekyll serve --port 5000 --incremental --livereload --destination docs
```

`--incremental` Incremental regeneration helps shorten build times by only
generating documents and pages that were updated since the previous build.

`--livereload` reload lively after every change
