# gkoumasd.github.io

Personal site of Dimitris Gkoumas.

| File | Page |
|---|---|
| `index.html` | About me (home page) |
| `ai-under-the-hood.html` | AI Under the Hood: study notes |
| `assets/images/profile.jpg` | Profile photo: the page loads `assets/images/square.jpg` from the live site |

## Publish on GitHub Pages

1. Copy these files into the root of the `gkoumasd.github.io` repository, replacing the old `index.html`. Keep the existing `assets/` folder for the photo.
2. Commit and push to the default branch:
   ```bash
   git add index.html ai-under-the-hood.html README.md
   git commit -m "New about page and AI Under the Hood notes"
   git push
   ```
3. The site updates at https://gkoumasd.github.io/ within a minute or two.

Both pages are self-contained HTML. They load Google Fonts and KaTeX (for equations) from public CDNs, and need no build step.
