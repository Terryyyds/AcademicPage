# Profile completion and release checklist

Prepared 22 October 2026 against Terryyyds/AcademicPage master at `fa525dd52481000b6254b920c4faab4d6ed52d42`.

## Confirmed and source boundaries

- The owner confirms publication and presentation of the PACIS work.
- The [AIS proceedings record](https://aisel.aisnet.org/pacis2026/dig_sec/dig_sec/10/) verifies the byline, complete-paper status, paper number and recommended citation. Use the full official title, ending in “Small and Medium Enterprises”.
- The [conference program](https://pacis2026.aisconferences.org/events/program-schedule/) places paper 1766 on 8 July 2026 in Jakarta. This is a scheduled date; completed presentation is based on the owner's confirmation.
- The [arXiv record](https://arxiv.org/abs/2605.18901) verifies the preprint identifier. Its DOI identifies the preprint, not a separately verified proceedings DOI.
- The University of Canterbury appears as the paper affiliation. Do not infer a degree, enrollment status or current employment from it.
- The owner supplied [LinkedIn](https://www.linkedin.com/in/yu-deng-396901303/) as the professional source. Direct access returned HTTP 999/robots restrictions. Public search-index snapshots of the exact profile were readable: [New Zealand snapshot](https://nz.linkedin.com/in/yu-deng-396901303) and [China snapshot](https://cn.linkedin.com/in/yu-deng-396901303). These are self-reported, indexed evidence, not live profile or issuer verification. The snapshots differ in recency and visibility.
- School names and profile-listed years, three selected certifications, the security assessment project, and the volunteer Swift teaching role are used only within the visible fields. No degree or employment title is inferred. The 2026–present entry requires current enrollment confirmation.

## Required owner details

- [ ] Confirm preferred public name. This patch uses the scholarly byline “Yu Deng”.
- [ ] Confirm the two LinkedIn-listed education entries and supply exact degrees, fields, attendance dates, completion status and current enrollment. Do not infer a Sanda University degree from an award entry.
- [ ] Supply current affiliation and employment history with dates and responsibilities.
- [ ] Supply technical tools, certifications and proficiency claims that can be supported.
- [ ] Confirm teaching and mentoring roles, subjects, service scope and contact method. No student outcomes, years of experience or paid services are claimed.
- [ ] Supply an approved portrait, public email, location, Google Scholar, ORCID and any additional personal profile links. The supplied LinkedIn URL is included; empty configuration fields intentionally hide other links.
- [ ] Add a public CV PDF and presentation slides only when available; there are no download links to missing files.
- [ ] Verify a proceedings DOI/page range before adding either; neither is required to cite the existing AIS record.

## Before deployment

- [ ] Review all visible “to be confirmed” text in About, both CV pages and Teaching; complete or remove the pending sections before the public release.
- [ ] Confirm hosting destination. `url: https://terryyyds.github.io` and `baseurl: /AcademicPage` are proposed settings for this project repository, not proof of an existing website. A root user site or custom domain requires different values.
- [ ] Confirm GitHub Pages source branch/folder or Actions workflow in repository settings. The existing scrape_talks workflow generates maps; it is not a Pages deployment workflow.
- [ ] In a full checkout with Ruby/Bundler, run `bundle install` and `bundle exec jekyll build --trace`. This patch has not been verified with a complete Jekyll build.
- [ ] Preview at `/AcademicPage/`, including About, Publications, the publication detail, Talks, the presentation detail, `/cv/`, `/cv-json/`, `/teaching/`, navigation, redirects and 404 behavior.
- [ ] Check desktop/mobile sidebar without a portrait, citation formatting, external links, sitemap.xml, feed.xml and canonical URLs.
- [ ] Verify excluded demo pages, sample PDFs/BibTeX and map artifacts are absent from `_site`; hiding a navigation item alone does not suppress a page.
- [ ] Keep the two CV representations consistent. Before using `scripts/update_cv_json.sh`, review its parser output: headings and schema may not preserve every manual field.
- [ ] Publication/talk TSV inputs now contain headers only. The new Markdown records are authoritative; populate and review generator inputs before using them.
- [ ] If maps are re-enabled, rebuild from the real talk record; old map assets are excluded from publication.
- [ ] After an authorized release, verify the actual public URL and Pages build status. Applying the patch changes source content only.

## Architecture and template content

Layouts, styles, JavaScript, collection definitions, plugin configuration and the template license remain in place. Fictional publications, talks, teaching entries, portfolio items and blog posts are removed. Demo guide/legal pages, development inputs, sample files and old maps are excluded from site output while remaining in the repository. Template attribution in README and LICENSE should be retained.
