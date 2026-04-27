# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static HTML website for GreenSuite (greensuite.ai), hosted on GitHub Pages with a custom domain managed via Cloudflare DNS.

## Hosting & Deployment

- **Host:** GitHub Pages, repo `greensuite-ai/greensuite-website`, branch `main`
- **Domain:** `greensuite.ai` — DNS is on Cloudflare with A records pointing to GitHub Pages IPs, proxy set to **DNS only (gray cloud)**
- **CNAME file:** `CNAME` in repo root maps the custom domain — do not delete it
- Deployment is automatic on every push to `main` — no build step required

## Structure

- `index.html` — single page, all CSS inline in `<style>`
- `images/` — static assets; logo at `images/greensuite.png`
- `CNAME` — required by GitHub Pages for custom domain

## Development

Open `index.html` directly in a browser to preview — no server or build tool needed.
