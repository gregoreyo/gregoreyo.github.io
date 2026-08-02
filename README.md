# gregoreyo.github.io

Personal site for Anthony Castaño — conference talks and projects, built with
[Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages at
[gregoreyo.github.io](https://gregoreyo.github.io).

Blog and contact form live separately at [anthonycastano.com](https://anthonycastano.com).

## Structure

```
_config.yml       Site settings, author info, collections
_layouts/         default.html (base layout), talk.html (talk pages)
_includes/        head.html, header.html, footer.html
_talks/           One markdown file per talk (collection, rendered at /talks/:path/)
assets/css/       Site stylesheet
assets/slides/    Slide decks and other talk downloads
index.md          Home page
talks.md          Talks index (/talks/)
projects.md       Projects index (/projects/)
```

## Adding a talk

Create a new file in `_talks/` named `YYYY-MM-DD-short-slug.md` with front matter:

```yaml
---
title: "Talk Title"
event: "Conference Name"
location: "City, ST"
date: YYYY-MM-DD
video_url: "https://..."        # optional
downloads:                       # optional
  - label: "Slides"
    url: "/assets/slides/talk.pdf"
---
A short description of the talk. This is used as the excerpt on the talks index page.
```

It will automatically show up on `/talks/`, sorted by date.

## Local development

```sh
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000`.
