# Copilot Instructions for 33villaroad.githhub.io

This repository is a Jekyll-based static site, using the Minima theme and GitHub Pages integration. Follow these guidelines to be productive as an AI coding agent:

## Architecture & Structure

- **Jekyll Site**: Source files are in the root and `_posts/`, with generated output in `_site/` (do not edit files in `_site/`).
- **Content**: Blog posts go in `_posts/` using the format `YYYY-MM-DD-title.markdown` with YAML front matter.
- **Pages**: Main pages (e.g., `about.markdown`, `index.markdown`, `404.html`) use YAML front matter and layouts defined by the theme.
- **Assets**: Static files (CSS, JS, images) are in `assets/` and `_site/assets/`.
- **Configuration**: Site-wide settings are in `_config.yml`. Theme and plugin settings are managed here.

## Developer Workflows

- **Local Development**:
  - Use `bundle exec jekyll serve` to build and preview the site locally. This auto-regenerates on file changes.
  - If you change `_config.yml`, restart the server to apply changes.
- **Dependencies**:
  - Ruby gems are managed via `Gemfile`. Run `bundle install` after changing dependencies.
  - Use `bundle exec` to ensure the correct gem versions are used.
- **Windows Support**:
  - Gems like `wdm`, `tzinfo`, and `tzinfo-data` are included for Windows compatibility.

## Project-Specific Patterns

- **Front Matter**: All posts and pages require YAML front matter for layout, title, and metadata.
- **Theme Customization**: To override theme defaults, create files in the root or `_layouts/` and reference them in front matter.
- **Plugins**: Managed in `Gemfile` and `_config.yml` under the `plugins:` key.
- **Exclusions**: Files and folders listed in `.gitignore` and `_config.yml`'s `exclude:` are not processed or committed.

## Integration Points

- **GitHub Pages**: Uses the `github-pages` gem for compatibility. Do not manually deploy; push to the repository for automatic build/deploy.
- **External Links**: Documentation and theme sources are referenced in `about.markdown` and `_posts/`.

## Examples

- **Creating a New Post**:
  - Add a file to `_posts/` named `YYYY-MM-DD-title.markdown` with appropriate front matter.
- **Customizing the Site**:
  - Edit `_config.yml` for global settings.
  - Add or override layouts in `_layouts/`.
- **Serving Locally**:
  - Run: `bundle exec jekyll serve`

## Key Files

- `_config.yml`: Site configuration
- `Gemfile`: Ruby gem dependencies
- `_posts/`: Blog post content
- `assets/`: Static assets
- `.gitignore`: Files/folders to exclude from git

---

For further details, see [Jekyll documentation](https://jekyllrb.com/docs/home) and [Minima theme](https://github.com/jekyll/minima).

If any section is unclear or missing, please provide feedback for improvement.
