# boogy-ai.github.io

The Boogy developer hub — the organization's GitHub Pages site, served at
**<https://boogy-ai.github.io/>**. A single static landing page that routes
developers and coding agents to the public MCP server (`https://api.boogy.ai/mcp`),
the SDK API reference, the web SDK, agent skills, the service catalog, and the platform.

Coding agents can bootstrap with zero install by connecting to the MCP server
(`claude mcp add boogy https://api.boogy.ai/mcp`): guidance + host-truth validation +
device-flow sign-in (`login` shows the user a link, returns a token — no CLI).

The endpoint is `api.boogy.ai`, not `boogy.ai` — `https://boogy.ai/mcp` is a 404
from the marketing site, and this file and the org profile both carried that
wrong host until 2026-09-29. `https://boogy.ai/llms.txt` is the maintained
source for agent-facing commands; copy from it rather than from memory.

## Editing

`index.html` is self-contained (inline CSS, Google Fonts, no build step).
Edit it and push to `main`; GitHub Pages redeploys automatically.

## Serving

GitHub Pages, source: **Deploy from a branch → `main` / root**
(Settings → Pages). `.nojekyll` makes Pages serve the files verbatim.

Per-repo project docs keep their own paths — e.g. the SDK rustdoc lives at
`boogy-ai.github.io/boogy-sdk/` and is unaffected by this site.
