# INNOEQX

Static, bilingual HTML pages. No build step is required.

## Pages

- [Homepage](index.html) redirects to the preferred
  [website design](INNOEQX_Website.html). Keep editing that original file;
  there is no duplicate copy of the design to maintain. The redirect uses a
  relative path for GitHub Pages project sites and preserves the query string
  and section fragment when JavaScript is enabled.
- [Executive report](INNOEQX_Executive_Report_EN_ES.html)
- [Service opportunity report](INNOEQX_Service_Opportunity_Report.html)

## Publish with GitHub Pages

1. Commit and push these files, including `index.html` and `.nojekyll`, to the
   branch you want to publish.
2. In the GitHub repository, open **Settings > Pages**.
3. Set **Source** to **Deploy from a branch**, select your branch and
   **/(root)**, then save.
4. Once deployment finishes, open the URL shown by GitHub Pages (normally
   `https://<username>.github.io/<repository>/` for a project repository).

The homepage redirects to `INNOEQX_Website.html`; the filename will appear in
the browser address bar. Both reports will also be publicly accessible by
their filenames. Review their contents before publishing.

## Before a production launch

- **The website contact form is a demo.** It does not send email, save a
  request, or contact a CRM. Connect a form-delivery service and replace the
  preview confirmation before accepting inquiries. GitHub Pages cannot run
  server-side form handlers.
- Replace the placeholder privacy/data-handling notice with your actual
  policy before collecting personal information.
- The website and service opportunity report load React 18.3.1 and ReactDOM
  from `unpkg.com`. They require JavaScript and access to that CDN; a blocked
  or unavailable CDN displays a load-error message instead of the page.
  The executive report has static HTML content, with JavaScript enhancements.
- After deployment, smoke-test the homepage, language switches, section links,
  and mobile layout at the real GitHub Pages URL. Local preview checks do not
  verify the repository's GitHub Pages configuration or deployment.
