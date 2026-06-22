# boogy-ai.github.io

The Boogy developer hub — the organization's GitHub Pages site, served at
**<https://boogy-ai.github.io/>**. A single static landing page that routes
developers and coding agents to the public MCP server (`https://boogy.ai/mcp`),
the SDK API reference, agent skills, the service catalog, and the platform.

Coding agents can bootstrap with zero install by connecting to the MCP server
(`claude mcp add boogy https://boogy.ai/mcp`): guidance + host-truth validation +
device-flow sign-in (`login` shows the user a link, returns a token — no CLI).

## Editing

`index.html` is self-contained (inline CSS, Google Fonts, no build step).
Edit it and push to `main`; GitHub Pages redeploys automatically.

## Serving

GitHub Pages, source: **Deploy from a branch → `main` / root**
(Settings → Pages). `.nojekyll` makes Pages serve the files verbatim.

Per-repo project docs keep their own paths — e.g. the SDK rustdoc lives at
`boogy-ai.github.io/boogy-sdk/` and is unaffected by this site.
