# Nøyra Labs

> Tools for teams, organizations and communities on Discord.

Nøyra Labs builds the **Nøyra Suite**: four products that run alongside your Discord server, share one sign-in, and use your server's own members and roles. Each product keeps its own data, and everything runs on Cloudflare.

**Website:** [noyralabs.com](https://noyralabs.com) · **Guides:** [docs.noyralabs.com](https://docs.noyralabs.com) · **Account:** [account.noyralabs.com](https://account.noyralabs.com)

---

## The Nøyra Suite

| Product | What it does | Site |
| --- | --- | --- |
| **Docket** | Ticket management: typed private-thread tickets, staff notifications, automatic transcripts and customer feedback, configured from one dashboard. | [docket.noyralabs.com](https://docket.noyralabs.com) |
| **Crew** | People management: roles imported from Discord, service records, org charts, shifts and activity, jobs and applications, requests and leave. | [crew.noyralabs.com](https://crew.noyralabs.com) |
| **Sensa** | Employee feedback: anonymous surveys and messages, with results only shown for groups of five or more. | [sensa.noyralabs.com](https://sensa.noyralabs.com) |
| **Aptio** | Training, exams and forms: courses marked on the server, with roles given automatically when someone passes. | [aptio.noyralabs.com](https://aptio.noyralabs.com) |

### One account

Sign in once with Discord at [account.noyralabs.com](https://account.noyralabs.com) to use every product. From there you can sign out everywhere, or delete your account and its data from every product at once.

### Client work

Alongside the Suite, we build custom tools for clients. See [noyralabs.com](https://noyralabs.com) for consulting.

---

## How we build

- **Discord is the source of truth.** People are their Discord account and organizations are their Discord server. Permissions follow current Discord roles and are checked on the server for every action.
- **Separate by design.** Each product and each organization keeps its own data, and one organization can never reach another's.
- **Privacy first.** Sign-in tokens are never stored, sessions are stored only as hashes, and Sensa's anonymity rules are enforced on the server.
- **Cloudflare-native.** Workers, Durable Objects, D1 and R2, with strict security headers and no servers to patch.

## Tech stack

| Category | Technologies |
| --- | --- |
| **Languages** | TypeScript |
| **Web** | Astro, Svelte 5, React islands, Tailwind CSS, DaisyUI |
| **Backend** | Cloudflare Workers, Hono, Zod |
| **Data** | Durable Objects (SQLite), D1, R2 |
| **Discord bot** | Sapphire Framework, Discord.js, Docker |
| **Testing** | Vitest (in workerd), Playwright, axe-core |
| **Tooling** | pnpm, ESLint, Prettier, GitHub Actions |

---

## Security

Please don't open public issues for security problems. Report them privately to Nøyra Labs.

<div align="center">

**Built by Nøyra Labs**

</div>
