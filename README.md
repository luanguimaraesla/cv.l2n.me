# CV - Luan Guimarães

Personal CV/Resume website built with Hugo and deployed via GitHub Pages.

Live site: https://cv.l2n.me

## Prerequisites

- [Hugo](https://gohugo.io/) (Extended version)
- Git

## Setup

Clone the repository and initialize the theme submodule:

```bash
git clone <repository-url>
cd cv.l2n.me
git submodule update --init --recursive
```

## Local Development

Start the Hugo development server:

```bash
hugo server
```

Or run on a specific port:

```bash
hugo serve -p 3000
```

The site will be available at http://localhost:1313 (or the specified port).

## Configuration

All content is configured in `config.toml`. Update the following sections:

- `[params.profile]` - Name, tagline, avatar
- `[params.contact]` - Contact information
- `[params.skills]` - Technical skills
- `[params.experience]` - Work experience
- `[params.education]` - Educational background
- `[params.projects]` - Notable projects
- `[params.social]` - Social media links

## Building for Production

Generate the static site:

```bash
hugo
```

The built site will be in the `docs/` directory, which is configured for GitHub Pages deployment.

## Deployment

This site is configured to deploy via GitHub Pages from the `docs/` directory on the `master` branch.

After making changes:

1. Update `config.toml` with your content
2. Build the site: `hugo`
3. Commit and push:
   ```bash
   git add .
   git commit -m "Update CV content"
   git push
   ```

Changes will be live at https://cv.l2n.me within a few minutes.

## Theme

This site uses the [Hugo DevResume Theme](https://github.com/cowboysmall-tools/hugo-devresume-theme) as a git submodule.

Theme customizations are in `layouts/partials/` to override default theme behavior.

## Troubleshooting

### Theme not loading

If you see errors about missing templates, ensure the theme submodule is initialized:

```bash
git submodule update --init --recursive
```

### Changes not appearing

1. Rebuild the site: `hugo`
2. If running the dev server, stop it (Ctrl+C) and restart: `hugo server`
3. Clear your browser cache

## License

Content: © Luan Guimarães. All rights reserved.

Theme: See [theme license](themes/hugo-devresume-theme/LICENSE.md).
