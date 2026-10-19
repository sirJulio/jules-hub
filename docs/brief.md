# Jules Hub — brief

Julio's online front door. The hub is a public landing page only: it offers a choice between his professional site and his project portal, and links to each. It does not manage anything itself.

## Current state (20 Oct 2026)
- Redesigned as a landing page: a title, one line, and a clean choice between two destinations, the professional site and the project portal.
- Static: `index.html` and `styles.css` only, with no JavaScript. Each choice shows "Opening soon" until its site has an address; see the README for turning it into a link.
- The earlier departures-board design (one row per project, with JH codes) is retired. The private claude.ai mockup at https://claude.ai/artifact/Y2ysMWs8dVgDEX95wCnUfn now shows the landing page.
- - Live at https://jules-hub.pages.dev (Cloudflare Pages, deploys from main).

## Destinations
| Destination | For | Status |
|---|---|---|
| Professional site | Employers and clients; includes the animated timeline idea | Planned |
| Project portal | Invited collaborators; manages all projects and includes the think tank | Planned |

Neither has a public address yet.

## Decisions
- The hub lives in the GitHub repo `jules-hub` and is built further in VS Code with Claude Code.
- The hub stays simple and static, with no build step. Host: Cloudflare Pages, connected to the repo (Pages rather than Workers for now; revisit Workers when the portal needs server functions).
- The professional site can be static too: its animated timeline runs in the browser from a data file.
- The project portal and professional site are separate apps, each with its own repo, launched from the hub.
- This repo is the source of truth for code and shared docs. The claude.ai Project "Jules Hub" is for discussion.
- The innovation catalogue becomes the **think tank**, a feature of the project portal rather than a hub section or a separate app. Ideas are logged and discussed there until they become projects; each idea links to the project it became, and each project to the idea it started as.
- All individual projects (podcast app, Institutional Intoxication, intellectual journal, Übermensch and future ones) are managed in the project portal, not listed on the hub. The hub offers only the two destinations; a project with its own public presence could be added later.
- Think tank participants: Julio, people he invites, and Claude as a participant in discussions.
- The portal, including the think tank, is private by default and invite-only. The hub only links to it.

## Open questions
- Domain name?
- Which address do employers and clients get: the hub, or the professional site directly?
- Portal: build first as a claude.ai artifact (private, invite by sharing, shared data, Claude built in) or go straight to a standalone app (own sign-in, database, and a server holding an Anthropic API key)?
- Portal: do thinking partners and paying clients see the same spaces, or does each project/idea have its own invite list?

## Workflow
- Discuss and decide in chat → record decisions in this file.
- Build in Claude Code → commit to the repo.
- Attach the repo to chat when reviewing code.
