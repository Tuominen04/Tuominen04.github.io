# My personal portfolio website

Go check it out: [https://tuominen04.github.io](https://tuominen04.github.io/)

Portfolio of Arttu Tuominen, a software developer focused on quality, test automation and observability (C#/.NET, CI/CD, OpenTelemetry, Azure, Rust, AI agents and MCP).

Built with [Jekyll](https://jekyllrb.com/) on the [al-folio](https://github.com/alshedivat/al-folio) starter and hosted on GitHub Pages.

## Where the content lives

| What                          | File                                                                                          |
| ----------------------------- | --------------------------------------------------------------------------------------------- |
| About page (home)             | `_pages/about.md`                                                                             |
| Projects                      | `_projects/*.md` (card order is the `importance` value, lowest first)                         |
| CV page                       | `assets/json/resume.json` (JSON Resume format, loaded via `jekyll_get_json` in `_config.yml`) |
| CV PDFs                       | `assets/pdf/arttu_tuominen_cv_en.pdf`, `assets/pdf/arttu_tuominen_cv_fi.pdf`                  |
| Site description and keywords | `_config.yml` (`description`, `keywords`)                                                     |
| CV page styling               | bottom of `assets/css/main.scss`                                                              |

When the CV changes, replace both PDFs and update `assets/json/resume.json` so the CV page matches.

## Run locally

```bash
bundle install
bundle exec jekyll serve      # http://localhost:4000/
bundle exec jekyll build      # one-off build to _site/
```

`baseurl` is empty in `_config.yml`, so the site is served at the root. Restart the server after editing `_config.yml`. Deployment is automatic: pushing to `main` runs the GitHub Actions deploy workflow.

For maintainer and agent notes see [AGENTS.md](AGENTS.md) and [CLAUDE.md](CLAUDE.md).
