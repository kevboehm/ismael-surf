# Ismael Araya — Surf Lessons

Simple link page for surf lessons in Costa Rica (WhatsApp + Instagram).

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `ismael-surf` or use the same name as your GitHub username for `username.github.io`).
2. Push this folder:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git branch -M main
   git push -u origin main
   ```
3. In the repo: **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Branch: **main**, folder: **/ (root)**. Save.
6. The site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/` (or `https://YOUR_USERNAME.github.io/` if the repo is `username.github.io`).

## Connect Your Namecheap Domain

After the site is live on GitHub Pages:

1. In **Namecheap**: Domain List → **Manage** next to your domain → **Advanced DNS**.
2. Add these records (remove or replace any existing A records for `@` if needed):

   | Type  | Host | Value              |
   |-------|------|--------------------|
   | A     | @    | 185.199.108.153    |
   | A     | @    | 185.199.109.153    |
   | A     | @    | 185.199.110.153    |
   | A     | @    | 185.199.111.153    |
   | CNAME | www  | YOUR_USERNAME.github.io |

   Replace `YOUR_USERNAME` with your GitHub username.

3. In **GitHub**: repo → **Settings → Pages**.
4. Under **Custom domain**, enter your domain (e.g. `yourdomain.com`).
5. Save, then check **Enforce HTTPS** once the domain is verified.
6. Wait 10–30 minutes for DNS to propagate.

Your site will be available at `https://yourdomain.com` and `https://www.yourdomain.com`.
