# Purpose
Static Nuts Tips website with legal/support pages, app links, and Apple association endpoints.

# Layout
- Root: landing page, legal HTML pages, advertising declaration, domain and hosting configuration.
- `.well-known/`: Apple app-site association endpoint; retain the root copy too.
- `app/`: app download landing page.
- `open/`: app-opening and App Store fallback page.
- `support/`: support page.

# How to test
No test command, package manifest, or test suite is supplied by this repository or move list.
Diagnostic command: `npm.cmd --offline test` (run from the repository root).
Confirmed FAIL: package.json is absent (ENOENT); no repository tests could run.

# What is live and how it deploys
`CNAME` names nutstips.com; HTML pages link to that domain.
`vercel.json` configures social-path rewrites and both Apple association endpoint headers.
Actual live hosting, deployment trigger, branch, and VPS/cron involvement: UNSURE.
No README or supplied cron inventory establishes the current deployment procedure.

# Rules
- Agents must never touch live databases, VPS systems, secrets, or deployments.
- Never push; Claude owns deployments and reviews/commits this reorganization.
- Keep temporary files outside this repository.
- Preserve published HTML paths and both Apple association endpoints.
- Only perform explicitly authorized repository changes; do not access the network for this task.
