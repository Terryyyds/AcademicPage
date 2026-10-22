# Maintaining the academic profile

The public profile was refreshed on 22 October 2026 from the owner's two supplied CVs and the official PACIS proceedings and arXiv records.

- `_data/cv.json` is the shared source for both CV routes, the Projects page and the Teaching page.
- `_includes/cv-template.html` renders the two CV routes from the same data.
- Update `_pages/about.md` and `_config.yml` when changing the biography, affiliation or contact email.
- `_publications/` distinguishes conference publications from preprints. Follow the latest authoritative byline and title for each public version.
- Exact months and titles that differ between source CVs are not reconstructed. Keep the supported year-level dates unless the owner supplies a correction.
- Do not upload the source CV PDFs or certificate scans. Maintain the website content directly and use only approved public profile assets.
- Keep sample/demo exclusions in `_config.yml`. The existing `master` branch/root GitHub Pages source publishes changes automatically.
- Check the Pages build result and the live About, Research, CV, Projects and Teaching routes after a change.
