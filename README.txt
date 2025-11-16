AustralianPoetry Jekyll site (Magazine theme)
-----------------------------------------------
This Jekyll site is pre-configured for GitHub Pages. To publish:

1. Create a new GitHub repository (public) named: yourusername.github.io OR any repo and enable Pages.
2. Upload the contents of this folder to the repository root.
3. Ensure _config.yml has 'url' set to https://australianpoetry.com
4. Commit and push. GitHub Pages will publish the site (use main branch or gh-pages depending on settings).
5. To use a custom domain (AustralianPoetry.com):
   - In your GitHub repo settings -> Pages -> Custom domain: add 'australianpoetry.com'
   - GitHub will provide DNS records (or use an A record to GitHub Pages IPs and a CNAME for www)
   - Alternatively add a CNAME file (already included) and set GoDaddy DNS: 
       A @ -> 185.199.108.153 (and other GitHub Pages IPs) OR follow GitHub's instructions.
6. After DNS updates, GitHub will issue SSL certificate automatically.

Notes:
- This is a static Jekyll magazine-style site with collections: poets, poems, articles.
- Edit markdown files in _poets, _poems, and _posts/_articles to update content.
- The contact form uses a mailto fallback; consider using a form service for a working backend.
