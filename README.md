# Clearpath Demo

Try **[Clearpath](https://clearpath-sandy.vercel.app)** end to end — per-deploy accessibility
regression monitoring that posts a diff straight into your pull requests.

This repo is a tiny sample site (`index.html`) with a few intentional accessibility issues, plus
a GitHub Action that runs Clearpath on every push and pull request.

## Test it in 4 steps

1. **Create a free Clearpath account** at https://clearpath-sandy.vercel.app and add a project.
2. Copy your project's **ingest token** and add it to this repo:
   *Settings → Secrets and variables → Actions → New repository secret* →
   name `CLEARPATH_INGEST_TOKEN`.
3. **Open a pull request** — edit `index.html` (e.g. add `alt="..."` to the image, or fix the
   low-contrast text) and open a PR.
4. Watch the **Accessibility** check run. The result appears as a status check, and — once you've
   installed the [Clearpath GitHub App](https://github.com/apps/clearpath-a11y) and linked the
   installation in your project settings — as a PR comment with the full diff.

## What you'll see

- A per-deploy diff: **new**, **worsened**, and **fixed** issues since the last scan.
- A merge-blocking check (configurable in your project settings: off / new / new-or-worsened).
- A live trend of your accessibility score in the dashboard.

CI scans are **unlimited** on every plan — the check runs in your runner, so usage stays flat.

---
A [QAShift](https://www.qashifthq.com) product.
