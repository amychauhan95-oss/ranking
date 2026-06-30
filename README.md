# 🇺🇸 USARemoteJobs.io — 2,000,000 Remote Jobs

A full job portal with **2,000,000 individual remote job pages** for USA-based companies, open to applicants worldwide.

## Features

- ✅ 2,000,000 unique job pages (/jobs/1 → /jobs/2000000)
- ✅ All jobs 100% Remote — open to 100+ countries
- ✅ JSON-LD JobPosting schema with applicantLocationRequirements
- ✅ 2,000 XML sitemap files + sitemap index
- ✅ robots.txt, pagination, REST API
- ✅ Zero database — deterministic generation
- ✅ Deployed on Cloudflare Pages

## Deploy to Cloudflare Pages

1. Push this repo to GitHub
2. Go to [Cloudflare Dashboard](https://dash.cloudflare.com)
3. Pages → Create a project → Connect to Git
4. Select your repository and deploy
5. Add environment variable: SITE_URL = https://your-domain.com

## URL Structure

| URL | Description |
|-----|-------------|
| `/` | Home page |
| `/jobs` | All jobs (paginated) |
| `/jobs/:id` | Individual job (1–2,000,000) |
| `/sitemap.xml` | Sitemap index |
| `/sitemap-*.xml` | Individual sitemaps |
| `/robots.txt` | robots.txt |
| `/api/jobs` | JSON API |

## Tech Stack

- **Runtime**: Cloudflare Workers / Pages
- **Framework**: Vanilla JS
- **Data**: Deterministic (no database)
- **Deploy**: Cloudflare Pages