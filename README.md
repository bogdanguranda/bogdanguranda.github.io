# bogdanguranda.github.io

Personal website built with Jekyll (GitHub Pages).

## Prerequisites

- macOS (instructions below use the Terminal)
- Ruby (recommended: Ruby 2.7+)
- Bundler (managed via the project's `Gemfile`)

If you use `rbenv` or `rvm` prefer installing Ruby via those tools to avoid system-wide changes.

## Install dependencies

Open a terminal in the project root and run:

```bash
# install bundler if you don't have it
gem install bundler

# install gems from Gemfile
bundle install
```

## Run locally

To serve the site locally with live-reload:

```bash
bundle exec jekyll serve --livereload
# open http://127.0.0.1:4000 in your browser
```

To build the static site to `_site`:

```bash
bundle exec jekyll build
```

Stop the server with `Ctrl+C`.

## Optional: Docker

If you prefer Docker (no Ruby install):

```bash
docker run --rm -v "$PWD":/srv/jekyll -p 4000:4000 jekyll/jekyll jekyll serve
```

## Notes

- The site source is in the repository root (`_layouts`, `_includes`, `_pages`, etc.).
- The generated site is placed in the `_site` folder after a build/serve.

If you'd like, I can also add a short `Makefile` or update the `Gemfile` to lock a Ruby version.
