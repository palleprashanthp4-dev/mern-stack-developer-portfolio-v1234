# Palle Prashanth Portfolio

Static, single-page portfolio built with HTML, CSS and JavaScript and deployed on Vercel.

## SEO implementation report

- Added a descriptive page title, unique meta description, requested name/role keyword phrases, author and index/follow directives.
- Added the canonical URL and Open Graph and Twitter Card metadata using the existing portfolio portrait.
- Added Schema.org `Person` JSON-LD with the supplied name, professional title, website, LinkedIn and GitHub profiles.
- Added root-level `robots.txt` and `sitemap.xml`. The portfolio is one public page; section links are in-page anchors, not separate pages.
- Retained the existing About, Learning, Projects, Contact content, social profiles, project links and contact details. Updated the main heading to identify Palle Prashanth as a MERN Stack Developer and corrected heading levels without changing their visible text otherwise.
- Added descriptive portrait alt text, intrinsic image dimensions, high priority for the hero portrait, lazy loading for the below-the-fold portrait, font/CDN preconnects and a keyboard-accessible skip link.
- Existing portfolio artwork and styles remain in place; no build tooling or separate application framework was introduced.

## Google Search Console

1. Deploy these changes to the existing Vercel project and confirm the canonical site URL is live.
2. Open [Google Search Console](https://search.google.com/search-console/) and add the site as a **URL-prefix property** for `https://mern-stack-developer-portfolio-v123-pearl.vercel.app/`. Alternatively, use a Domain property if you control and can verify the relevant DNS domain.
3. Complete the verification method Search Console offers. For URL-prefix verification, it may provide an HTML file or a meta tag; publish that exact file/tag as supplied by Google. No verification token is prefilled in this project.
4. In Search Console, open **Sitemaps**, submit `sitemap.xml`, and check for a successful read.
5. Use **URL Inspection** for `https://mern-stack-developer-portfolio-v123-pearl.vercel.app/`, run **Test live URL**, then choose **Request indexing** if the page is available.
6. Check indexing and enhancements periodically. Google controls crawling, indexing, snippets and ranking; submission does not guarantee inclusion or a particular position.

## Pre-deployment verification checklist

- [ ] Confirm the Vercel production URL remains `https://mern-stack-developer-portfolio-v123-pearl.vercel.app/`.
- [ ] Deploy `index.html`, `style.css`, `main.js`, `profile_img.png`, `robots.txt` and `sitemap.xml` from the project root.
- [ ] Open `/`, `/robots.txt` and `/sitemap.xml` on the deployed site and confirm each returns successfully.
- [ ] Confirm the canonical, Open Graph, Twitter and JSON-LD URLs all use the production hostname.
- [ ] Validate the rendered page, mobile navigation, theme switch, contact form, project links and portrait after deployment.
- [ ] Test the page with Google Search Console URL Inspection and submit the sitemap.
