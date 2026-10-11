# CineHype for CloudStream

A single-site CloudStream provider project for `https://cinehype.sc`.

## Important status
This is a GitHub-uploadable **starter project**, not a verified working CineHype provider yet. The site did not expose readable page HTML to the inspection tool, so its catalog selectors, episode structure, and video source behavior could not be verified. The provider currently includes safe placeholders and does not scrape or resolve video streams. Complete the site-specific parsing only for content you are authorized to access and redistribute.

## Upload to GitHub
1. Download and unzip this folder.
2. Create a new **public** repository on GitHub named `CineHype-CloudStream`.
3. On the repository page choose **Add file → Upload files**.
4. Upload all files and folders from this directory (not the outer ZIP).
5. Commit the upload.
6. Open the **Actions** tab and enable workflows if GitHub asks.

## Build
The GitHub Actions workflow uses Gradle to compile the provider. A successful build only verifies the starter code; it does not mean the CineHype catalog or playback has been implemented.

## Add to CloudStream
A source repository is not installable until a `.cs3` plugin package is built and published, and a valid `repo.json` points to that package. Do not add the placeholder `repo.json` to CloudStream expecting a working extension.

## Project structure
- `CineHype/` — the single CineHype provider module
- `.github/workflows/build.yml` — automated build
- `repo.json` — placeholder index, to be populated after publishing a real plugin package
