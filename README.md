# gregoreyo.github.io

This is Anthony Castaño's personal website. It's a simple, single-purpose site for sharing:

- **Talks** — slides, videos, and downloads from conferences I've spoken at
- **Projects** — things I've built
- **About** — a bit about my background and how to find me elsewhere online

The blog and contact form live separately at [anthonycastano.com](https://anthonycastano.com); this site is just the talks/projects/about side of things.

It's built with [Jekyll](https://jekyllrb.com/) and hosted for free on [GitHub Pages](https://pages.github.com/) at [gregoreyo.github.io](https://gregoreyo.github.io).

## Adding a new talk

New talks go in the `_talks/` folder as a markdown file and show up automatically on the Talks page, sorted by date. Copy an existing file in that folder as a starting point for the front matter (title, event, date, links, etc.).

## Running it locally

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` in a browser.
