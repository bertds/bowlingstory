# blog_bowling (bowlingstory)

## What it does
A single-page static blog that tells a tongue-in-cheek, fictional story, "The Lakenhallen Invitational: Silicon vs. Steel in Old Leuven": a bowling tournament in the Leuven Lakenhallen between a human ("Superman") and an AI-themed rival, written as an AI-industry satire. `index.html` loads `story.md` content with marked.js, renders LaTeX with MathJax, and is pre-rendered/SEO-optimised (meta tags, JSON-LD schema). It also ships LLM-discovery files (`llms.txt` distilled summary, `robots.txt`) as an experiment in making content readable by AI crawlers. Hosted via GitHub Pages with custom domain `blog.ccstudios.be` (`CNAME`).

## Install
```bash
git clone https://github.com/bertds/bowlingstory
cd bowlingstory
```
No build step, no dependencies, no API keys (CDN scripts: marked, MathJax, Google Fonts). Not a Python project, so no requirements.txt.

## Run
```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
Deploy: push to GitHub and enable Pages on the main branch (custom domain from `CNAME`; the canonical URL in `index.html` is https://bertds.github.io/bowlingstory/).

## Result / output
A styled one-page article with hero image `live_coverage.png`, standings and a LaTeX formula; plus `llms.txt` / `robots.txt` for crawlers.

## Status
Last activity: February 2026. Archived experiment (static site, finished).
