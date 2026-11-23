# Yunao Dong's homepage

Source for <https://chris-hornet-dong.github.io>, built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll).

## Where things live

| What                              | File                                                                    |
| --------------------------------- | ----------------------------------------------------------------------- |
| Site name, URL, feature flags     | `_config.yml`                                                           |
| Homepage (bio, education, awards) | `_pages/about.md`                                                       |
| Publications                      | `_bibliography/papers.bib` (`selected={true}` shows it on the homepage) |
| Publication thumbnails            | `assets/img/publication_preview/`                                       |
| Email / Scholar / GitHub icons    | `_data/socials.yml`                                                     |
| Photography page                  | `_pages/misc.md`, photos in `images/`                                   |

## Deploying

Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site and pushes it to the `gh-pages` branch.
In the repository settings, **Pages → Build and deployment → Source** must be "Deploy from a branch" with branch `gh-pages` / `(root)`.

## Local preview

With Docker: `docker compose up`, then open <http://localhost:8080>.
With Ruby 3.3: `bundle install && bundle exec jekyll serve`, then open <http://localhost:4000>.
