# jadia
Jadia n e wilson
# JNEW Artistry — Jadia N E Wilson (jnew_art)

This repository is a starter static website for Jadia N. E. Wilson (social: @jnew_art). It includes:

- Bio (home) page
- Galleries: Graphic, Photography, Illustration, Visual Arts, Murals
- Store page (PayPal / Cash App / Zelle links)
- Contact page with file upload via Formspree or Netlify Forms
- Example Stripe serverless function for card payments (do NOT include secret keys in the repo)

Live site (when published): https://jnewartistry.online

How to use
1. Upload your images to assets/images/:
   - logo.png
   - keyring1.jpg
   - keyring2.jpg
   - visual1.jpg
   - visual2.jpg
   - visual3.jpg
   - visual4.jpg

2. Update Formspree endpoint (contact form) or enable Netlify Forms:
   - For Formspree: replace action in contact form with your Formspree form ID.
   - For Netlify: remove action and add `data-netlify="true"` to the form tag.

3. Stripe (optional):
   - Deploy `functions/create-checkout-session.js` to Vercel or Netlify Functions.
   - Set environment variables `STRIPE_SECRET_KEY` and `STRIPE_PUBLISHABLE_KEY` in your host.

Deploying
- Quick & free: GitHub Pages (static content only; file uploads and serverless require other hosts)
- Recommended for forms & serverless: Netlify or Vercel (can host serverless Stripe function and accept file uploads)

Custom domain
- The repo contains a CNAME with `jnewartistry.online`. After enabling Pages, set DNS to point to GitHub Pages (A records or CNAME). See GitHub Pages docs.

Security & notes
- Do NOT commit secret keys. Use environment variables for Stripe or any secrets.
- The PayPal email displayed is: jadiawilson@outlook.com (replace if needed).
- Review Formspree / Netlify file upload limits and privacy settings before accepting client files.

If you want help pushing these files, say "Push instructions" and I’ll give step-by-step Git commands or guide you through the GitHub web uploads.
