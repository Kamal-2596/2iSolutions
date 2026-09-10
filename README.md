# 2iSolutions — GitHub Pages review website

This package contains the corrected website, optimized local images and crawler files. The page design and content are unchanged. No installation, API key or build command is needed.

## Publish using the GitHub website

1. Unzip this package on your computer.
2. Sign in to https://github.com/ and create a new Public repository. For a site at the domain root, name it YOUR-USERNAME.github.io, replacing YOUR-USERNAME with your actual GitHub username in lowercase. Select Add README when creating the repository.
3. In the repository, choose Add file > Upload files. Drag in the CONTENTS of the extracted folder: index.html, assets/, robots.txt, llms.txt and README.md. Keep the assets folder intact. Do not upload the ZIP itself or nest everything inside an extra parent folder.
4. Click Commit changes to save the upload on the main branch.
5. Open Settings > Pages. Under Build and deployment, choose Deploy from a branch. Select main and /(root), then click Save.
6. Wait for publishing to complete (GitHub says it can take up to 10 minutes). Refresh Settings > Pages and click Visit site. Share this website URL for review rather than the repository URL.
7. Your root site URL will be https://YOUR-USERNAME.github.io/. Use this HTTPS URL to test the videos and run Lighthouse.

An optional .nojekyll file is included to bypass Jekyll processing. If your file browser hides it, the other files still work with the default Pages build. You can also create it through Add file > Create new file, name it .nojekyll and commit it.

## If you already have a username.github.io website

Do not replace an existing website. Create a separate Public repository named 2isolutions-review and follow the same upload and Pages settings. Your review URL will be https://YOUR-USERNAME.github.io/2isolutions-review/. All image paths in this package work under that repository subpath.

For a project site, robots.txt is published inside /2isolutions-review/; search engines and some audits instead request /robots.txt at the hostname root. Managing that root crawler file requires the username.github.io repository or a separate custom domain. Preserve any existing root crawler rules. The llms.txt file can also be used within a subpath, although a particular audit may check only the domain root.

## Files

- index.html: complete responsive homepage with inline CSS, fonts and JavaScript.
- assets/: optimized WebP illustrations, client logos and video thumbnails.
- robots.txt: basic crawler rules for a newly hosted site.
- llms.txt: company and service resource index.
- .nojekyll: optional static-publishing marker.

## Playback and review

All three testimonials retain thumbnails and Play buttons. On HTTPS, Play opens the embedded video modal. If the browser blocks YouTube, a direct Watch on YouTube fallback appears. Local file previews open YouTube directly because local files do not provide a normal HTTP referrer. No YouTube player is requested until a visitor chooses Play.

Service, company and contact links deliberately continue to the existing 2isolutions.com pages. This package is the homepage redesign, not copies of those inner pages. Canonical metadata continues to point to the company homepage.

This produces a publicly accessible review page. No GitHub repository or live deployment has been created for you. Live YouTube playback and Lighthouse scores must be verified after you publish.

## Updating the review page

Upload the changed index.html or assets through Add file > Upload files and commit to main. GitHub Pages publishes the update automatically. Hard-refresh the page if the browser still shows a cached version.

## Official instructions

- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
