# JD Detailing Website

Free static website for JD Detailing. Built for GitHub Pages and custom domain `jddetailing.biz`.

## Files

- `index.html` — main website page
- `style.css` — website styling
- `CNAME` — custom domain file for GitHub Pages
- `.nojekyll` — helps GitHub Pages serve files normally

## How to publish on GitHub Pages

1. Create a new GitHub repository named something like `jd-detailing-site`.
2. Upload all files from this folder into the repository.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ root**
5. Click **Save**.
6. Under **Custom domain**, enter `jddetailing.biz`.
7. Save.
8. In GoDaddy DNS, point the domain to GitHub Pages.

## GoDaddy DNS for GitHub Pages

Add these A records for the root domain:

```
Type: A | Name: @ | Value: 185.199.108.153
Type: A | Name: @ | Value: 185.199.109.153
Type: A | Name: @ | Value: 185.199.110.153
Type: A | Name: @ | Value: 185.199.111.153
```

Add this CNAME record for www:

```
Type: CNAME | Name: www | Value: YOUR-GITHUB-USERNAME.github.io
```

Replace `YOUR-GITHUB-USERNAME` with your real GitHub username.

## Booking form note

GitHub Pages is static hosting, so it does not store form submissions by itself. This version uses an email form that opens the customer's email app. For a better free form, connect Formspree, Google Forms, or use Netlify Forms.
