# Siyi Teng — Single-page academic homepage

A self-contained Jekyll / AcademicPages-style homepage adapted from the provided site, with a left profile sidebar and blue non-underlined links. All content lives on **one page**; journal and conference papers are mixed together in the publications list.

## Main files

- `_pages/home.md`: Homepage with biography, research interests, publications, experience, academic services, teaching, and selected awards. Modify this file to update the CV content.
- `_data/navigation.yml`: Header links, all pointing to sections of `/`.
- `_config.yml`: Name, profile information, and deployment settings.
- `_includes/head/custom.html`: Site-specific styles.
- `files/papers/`: Three locally hosted paper PDFs.
- `images/favicon.svg`: Initials-style favicon.

All details under Experience, Academic Services, Teaching, and Selected Awards reflect the text supplied by the user in November 2026. The Outstanding Graduate award is deliberately shown **without a year**, as no award year was specified. The original site portrait is not reused; the sidebar shows an `ST` placeholder.

## Local preview

From this folder (with Ruby, Bundler, and Jekyll available):

```bash
gem install bundler
bundle install
bundle exec jekyll serve --livereload
```

Then visit http://127.0.0.1:4000/ . A standalone HTML preview is also supplied separately; unlike a full Jekyll build, the HTML preview has embedded simplified CSS for offline viewing.

## GitHub Pages

Copy the **contents** of this folder into the root of the intended GitHub Pages repository (rather than uploading the whole folder as a nested directory). Under repository Settings → Pages, enable deployment from the default branch and root. Keep `baseurl: ""` for a username.github.io site or custom domain; project-repository deployments may need root-relative PDF links updated.

There are no independent teaching, awards, journal, or conference pages. All original-owner content and tracking identifiers are omitted.
