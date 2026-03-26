# ray.pillers.us — Changes Ready to Push
_Prepared by Sofia, 2026-03-25. Review and push to GitHub._

## Files Modified

### `_config.yml`
- `title` → "Raymond Piller" (was "Ray Things")
- `repository` → `VertigoRay/ray.pillers.us` (was `VertigoRay/ltec5240.ray.pillers.us` — wrong repo!)
- `author.bio` → "Senior Security Architect at Baylor Scott & White Health..."
- `author.location` → "San Antonio, TX" (was "Ecuador")
- `author.email` → `ray@pillers.us` (was blank)
- Author links: email → `ray@pillers.us` (was stale UNT address); website → `vertigion.com`; removed Facebook; added LinkedIn
- `description` was already correct: "Senior Security Architect | Healthcare Cybersecurity | HIPAA & FDA Compliance"

### `_data/navigation.yml`
- Added nav links: About, Projects, Graduate Studies, Blog
- Was previously all commented out (no navigation!)

## Files Created

### `_data/projects.yml`
- Full project data: 6 personal repos + 7 UNT-CAS repos
- Used by `_pages/projects.md` via Liquid loops

### `_pages/projects.md`
- New /projects/ page — lists all repos with stars, forks, tags
- Two sections: Personal Projects + UNT-CAS org work

### `_pages/masters.md`
- New /masters/ page — Graduate Studies landing
- Lists all 5 LTEC courses; notes that subdomains redirect here
- Placeholder for content migration (LTEC repos → posts with `masters` category)

### `_pages/about.md`
- New /about/ page — full professional bio
- Lists focus areas: CyberArk, CrowdStrike, Proofpoint, XSIAM, HIPAA/FDA
- Links to /projects/ and /masters/

## To Push

```bash
cd /root/.openclaw/workspace-marco/projects/ray.pillers.us
git add -A
git commit -m "Portfolio modernization: professional bio, projects page, masters section, nav

- Update title, bio, location, email, links in _config.yml
- Fix stale repository reference (was ltec5240, now ray.pillers.us)
- Add navigation: About, Projects, Graduate Studies, Blog
- New /projects/ page: PSRedstone, PSWriteLog, CVE-2021-36934, QuserObject, ePOwerShell, Vagrant-AD-Lab, etc.
- New /masters/ page: LTEC5210-6800 grad studies landing page
- New /about/ page: BSWH, CrowdStrike, CyberArk, XSIAM, HIPAA/FDA focus areas"
git push origin master
```

## Still TODO (after push)
- [ ] Migrate LTEC blog posts from the 5 standalone repos into `/masters/` as tagged posts
- [ ] Set up DreamHost 301 redirects for ltec*.ray.pillers.us subdomains (Eitan)
- [ ] Review existing 15 posts — re-tag/categorize under `masters` where appropriate
- [ ] Screenshot/visual review with Ray before DreamHost redirects go live
