# Premed Atlas

A small, static hub for the three study apps:

| Display name | App |
| --- | --- |
| CHEM 105a | https://amirlobel-elinor.github.io/genchem-atlas/ |
| BISC 120/220 | https://amirlobel-elinor.github.io/genbio-atlas/ |
| Element Atlas | https://amirlobel-elinor.github.io/element-atlas/ |

## Upload to GitHub

1. Unzip `premed-atlas-github.zip` on your computer. Do not upload the ZIP itself.
2. Open the GitHub repository for the central **Premed Atlas** site (not one of the individual study apps). If you are creating a new hub, a repository named `premed-atlas` is suitable.
3. At the repository's top level, choose **Add file → Upload files**. Drag in all six extracted files, not their enclosing folder. If updating this hub, the files with matching names replace the previous versions after you commit.
4. Commit the upload to the publishing branch, usually `main`. Keep any unrelated files and any existing custom-domain `CNAME` file.
5. For a new GitHub Pages site: open **Settings → Pages**, choose **Deploy from a branch**, select `main` and **/(root)**, then **Save**. If this hub already uses that configuration, leave it in place.
6. Wait for the Pages deployment to finish, then use the site link shown in Settings → Pages. If the repository is `premed-atlas` under the account above, the expected URL is https://amirlobel-elinor.github.io/premed-atlas/ . This package does not publish it automatically.

All six files sit at the repository root; there are no subfolders or build steps:

| File | Purpose |
| --- | --- |
| `index.html` | Complete site, with embedded styles and illustrations |
| `favicon.svg` | Scalable browser-tab icon |
| `favicon.ico` | 16px, 32px, and 48px browser-icon fallback |
| `favicon-32.png` | 32px PNG browser icon |
| `apple-touch-icon.png` | 180px home-screen bookmark icon |
| `README.md` | These instructions |

## Preview and update

Open `index.html` in a browser to preview the site locally. Keep the icon files next to it. The separate `premed-atlas.html` artifact is a self-contained preview of the same design; it is not needed in the repository.

The site has no external fonts, libraries, tracking, account system, or build dependencies. All three cards open the supplied app URLs in new tabs. Each entire card is a link; its small feature labels are not separate buttons.

The footer's suggestion link opens the visitor's email app, addressed to `amirlobe@usc.edu`. It does not send automatically or collect submissions through a server.

The logo follows the saved Atlas app family: a framed **Pa** letter tile, matching the Ea and Ca tile structure and the framed B.a biology mark. Its violet face (#7360e5), raised edge, cyan medical plus, and gold sparkle use colors and tactile styling from the latest chemistry and element apps. The header, introductory illustration, and browser icons share this mark. Icon links include `?v=5` to help with cached favicons. If an older icon persists after a completed deployment, try a new tab or private window and check that all icon files were uploaded. Browser favicon caches may update separately from page content.

To edit the hub later, change the three card links and their text in `index.html`. Keep the visible course labels and accessible link names in sync. Updating this hub does not change any of the three linked apps.

GitHub Pages setup reference: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
