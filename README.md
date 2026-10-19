# Sun Scan

A simple, mobile-friendly scanlation-style website with a dark theme and blue accents. Built as a static site that can be hosted on GitHub Pages.

## Included
- Simple latest-updates list and series grid
- Search, genre filters, and sorting
- Series details and chapter list
- Vertical chapter-reader layout with placeholder panels
- Browser-local bookmarks and reading progress
- No build tools or package installation required

## Publish with GitHub Pages
1. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the root of your repository.
2. Commit the files to your `main` branch.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/(root)`, then save.
6. Wait for GitHub Pages to publish. The URL usually looks like `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

When you update the site, upload the changed files and commit again.

## Add a series
Open `app.js` and find `const SERIES = [` near the top. Copy a series object and change its `id`, `title`, `genres`, `status`, `chapter`, `updated`, `label`, `cover`, `orb`, `synopsis`, and `chapters` values. Each `id` must be unique.

## Add chapter images
The reader currently contains placeholder panels. To show real pages, add chapter images to your repository and update `renderReader()` in `app.js` to display them vertically. Only publish artwork, chapters, and translations you own or have permission to distribute.

## Limitations
This is a static front-end, not a full publishing system. Series and chapter lists are edited in `app.js`; there is no admin dashboard, database, or user login. Bookmarks and reading progress are saved only in the current browser. The demo series and reader panels are placeholders.
