# Brian K Chen — personal website

A static academic website ready for GitHub Pages. No installation, build step, framework, external fonts, or account credentials are required.

## Preview locally

Open `index.html` in a browser. The homepage, CV, styling, portrait, and work-in-progress disclosure work directly from the files. Paper links require an internet connection.

The CV page has a **Print / save PDF** button. Choose **Save as PDF** in your browser's print dialog to export it; turn off browser headers and footers for a cleaner result. This is a printable HTML CV, not a bundled PDF file.

## Upload to GitHub Pages

1. Sign in to GitHub and create a repository named `YOUR-USERNAME.github.io`, replacing `YOUR-USERNAME` with your GitHub username. A public repository works with GitHub Free.
2. Choose **Add file → Upload files**. Upload the **contents of this folder**, preserving the `assets` folder. `index.html` must be at the top level of the repository, not inside another `github-pages` folder. If using the ZIP, extract it first; do not upload the ZIP itself.
3. Commit the uploaded files to `main`.
4. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/ (root)**. Click **Save**.
5. GitHub will show your published URL, normally `https://YOUR-USERNAME.github.io/`. Publication can take a few minutes.

The empty `.nojekyll` file disables Jekyll processing. Include it when uploading (files beginning with a dot may be hidden in your file browser). If it is omitted, this plain HTML/CSS site can still be served by GitHub Pages.

You can also use a differently named project repository. All local links are relative, so the site works at `https://YOUR-USERNAME.github.io/REPOSITORY/` as well.

Official instructions:
- [Create a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [Configure the publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Files

```text
index.html           Homepage, publications, and current research
cv.html              Public, printable curriculum vitae
styles.css           Responsive layout, colours, typography, and print styles
cv.js                Print button for the CV
assets/profile.jpeg  Profile photo
assets/favicon.svg   BC browser-tab icon
.nojekyll            Disables Jekyll processing
README.md            These instructions
```

Upload only this folder's contents. The original résumé source in the parent folder is not part of the website package.

## Editing

- **About, contact, and research:** edit the corresponding sections of `index.html` in a text editor. Comments mark the main sections.
- **Publications:** duplicate an existing `<li class="publication">` block, then update the title, authors, venue, year, and links. Update the matching entry in `cv.html` too.
- **Submissions:** each manuscript is an `<li>` in the `manuscripts` list. Keep submission status distinct from accepted publications.
- **Work in progress:** edit the `project-list` entries and the project count in the disclosure heading.
- **CV:** edit `cv.html`; the print styles are at the end of `styles.css`.
- **Photo:** replace `assets/profile.jpeg`. Its framing is controlled by `.portrait img` in `styles.css`.
- **Appearance:** change the colour variables at the start of `styles.css`.
- **Profile links:** add your Google Scholar or GitHub profile once you have the exact URLs. No guessed profile links are included.
- **Dates:** update the homepage copyright year and the CV's updated date when needed.

## Content notes

- The website and public CV identify Brian K Chen as **Independent Researcher**.
- Content is based on the supplied résumé and About text. The public CV omits phone number, citizenship, and grades.
- PrefixMemory-Tuning is listed as **ICLR 2026**, matching the [ICLR 2026 listing](https://iclr.cc/Downloads/2026), [paper](https://arxiv.org/abs/2506.13674), and [coauthor's website](https://hu-tianyang.github.io/). The supplied résumé listed 2025.
- Published paper links point to arXiv, PMLR, OpenReview, or the journal. A public preprint was found for Speculative Correction. Other submitted manuscripts and ongoing projects are shown without invented links.
- Unpublished entries retain the supplied author lists.
- Structure was inspired by the supplied academic website reference; all site code here is original.

The entire homepage works without JavaScript. There are no analytics, cookies, remote font requests, or third-party scripts.
