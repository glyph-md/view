# Glyph web viewer

**https://glyph-md.github.io/view/**

Read a markdown file in any browser, or open a link that carries a whole
document. Files you open stay in your browser and are never uploaded; a shared
link holds the document itself, compressed into the part of the URL after `#`,
which browsers never send to a server.

The viewer is part of [Glyph](https://github.com/hamidfzm/glyph). Its source
lives there, in `src/web/`. This repository only publishes it.

## How it is published

`.github/workflows/deploy.yml` checks out `hamidfzm/glyph` at a given tag or
commit, runs `pnpm build:web`, and deploys `dist-web/` to GitHub Pages. Each
Glyph release starts it with the release tag. To redeploy by hand, run the
**Deploy** workflow from the Actions tab with the ref to build.

Report problems and suggest changes in
[hamidfzm/glyph](https://github.com/hamidfzm/glyph/issues).
