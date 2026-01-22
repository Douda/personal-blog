# Cloud Mastery Journey

A technical blog documenting my progression through cloud computing certifications, infrastructure automation, and DevOps practices.

## About This Project

This repository contains the source code for my personal blog at [boumanne.fr](https://boumanne.fr), where I document my cloud learning journey

The blog serves as both a knowledge repository and a platform for sharing insights with the cloud computing community.

## Technical Stack

- **Static Site Generator**: Hugo (v0.154.2+)
- **Theme**: [hugo-blog-awesome](https://github.com/hugo-sid/hugo-blog-awesome)
- **Hosting**: GitHub Pages
- **Deployment**: GitHub Actions (automated)
- **Domain**: boumanne.fr

## Deployment

### Automatic Deployment

The site automatically deploys to GitHub Pages via GitHub Actions on every push to the `main` branch.

Workflow: `.github/workflows/deploy.yml`

### Manual Build

Generate static files:

```bash
hugo --gc --minify
```

Output directory: `public/`

## Configuration

Site settings are managed in `config.toml`:

- Site metadata and SEO
- Author information
- Social media links
- Theme customization
- Menu structure

## Project Structure

```
blog-douda/
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions deployment
├── content/                # Markdown content
├── static/                 # Static assets (CNAME, images)
├── themes/
│   └── hugo-blog-awesome/  # Theme submodule
├── config.toml             # Hugo configuration
└── README.md
```

## Contributing

This is a personal blog, but I welcome:

- Constructive feedback on technical content
- Bug reports and issue submissions
- Suggestions for topics to cover
- Collaboration on cloud-related projects

## License

Blog content is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).

Code snippets and configuration files are available under the MIT License unless otherwise noted.

---

Built with Hugo. Deployed on GitHub Pages.
