# ingest-architecture-board (deploy mirror)

**Content source of truth**: [vibe-coding-stack](https://github.com/spacebuilder13/vibe-coding-stack) → `boards/ingest-architecture-board/` (edit `data/*.mmd` and `data/*.md` there).

This repo exists for **GitHub Pages**, **Giscus** (Discussions on *this* repo), and a thin deploy surface. After editing the board in vibe-coding-stack, sync here:

```bash
# from vibe-coding-stack clone (sibling folder = ingest-architecture-board)
rsync -av --delete boards/ingest-architecture-board/ ../ingest-architecture-board/
```

Then commit + push this repo.

## Live site

https://spacebuilder13.github.io/ingest-architecture-board/

## Local preview

```bash
python3 -m http.server 4173
```

## Giscus

Requires [giscus GitHub App](https://github.com/apps/giscus) installed on this repo. Category IDs live in `app.js`.
