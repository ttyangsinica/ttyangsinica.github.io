# Causality & Policy Evaluation Research Group website

This is a Jekyll website for GitHub Pages. It is designed so that most updates can be made by editing Markdown pages or YAML data files.

## Main pages

- `index.md`: home page
- `research.md`: research page
- `teaching.md`: teaching page
- `members.md`: members page
- `join-us.md`: recruitment page

## Data files

- `_data/working_papers.yml`: working papers
- `_data/publications.yml`: publications
- `_data/courses.yml`: current and past courses
- `_data/labor_economics_2026.yml`: detailed schedule for the Spring 2026 labor economics course
- `_data/members.yml`: lab members and alumni groups
- `_data/openings.yml`: recruitment items

## Updating the site manually

Edit the relevant `.md` or `.yml` file on GitHub, commit the change, and GitHub Pages will rebuild the site.

## Deploying

Create a GitHub repository named `ttyangsinica.github.io`, push these files to the `main` branch, then go to:

`Settings > Pages > Build and deployment > Source`

Choose `GitHub Actions`. The workflow in `.github/workflows/pages.yml` will build and deploy the site.

## Local preview

If Ruby and Bundler are installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.
