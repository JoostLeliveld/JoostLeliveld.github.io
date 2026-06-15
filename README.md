# Joost Leliveld Personal Website

Source code for my personal portfolio at:

https://joostleliveld.github.io/

The site is built with Hugo Blox and hosted with GitHub Pages. It is structured around engineering case studies in robotics, computer vision, sensor fusion, learning-based control, sim-to-real reinforcement learning, and embedded AI systems.

## Main Content

- `content/_index.md` - homepage sections and project ordering.
- `data/authors/me.yaml` - profile, links, education, experience, skills, and interests.
- `content/projects/` - portfolio case studies.
- `content/publications/` - thesis/research/report entries.
- `content/blog/` - technical notes.
- `assets/media/authors/me.png` - profile image used by the author profile.
- `static/` - files copied directly to the public site root, including Google verification files.

## Local Development

```bash
pnpm run dev
```

Build the production site and Pagefind search index:

```bash
pnpm run build
```

## Deployment

The repository uses GitHub Actions to build and deploy the site to GitHub Pages when changes are pushed to `main`.

## Notes

Project pages should make ownership clear:

- Link public repositories when code is available.
- Mark team projects as team projects.
- Explain my specific contribution.
- For private code, show architecture, methods, results, screenshots, videos, and lessons without exposing private repositories.
