# Shri Purna Chikans — customised website

A responsive, premium-styled one-page website for Shri Purna Chikans, a Lucknow-based Chikankari business. It includes the supplied phone/WhatsApp number, public shop address, Instagram link, the business story and the selected product categories.

## Files
- `index.html` — page content, SEO metadata and local-business structured data
- `styles.css` — responsive design
- `script.js` — mobile navigation and footer year
- `CNAME` — custom domain (`shripurnachikans.com`)
- `assets/products/` — add your own product photos here
- `assets/images/` — place your logo here when ready to add it to the page

## Before publishing
1. **Logo and product photographs:** you said you have a logo, but no logo file or product photographs were attached to this message. The site currently uses a text monogram and clearly marked photo placeholders. Add your actual logo and real product images before launch.
2. **Contact details:** the supplied business email `shripurnachikans@gmail.com` is included as a clickable email link and in the local-business structured data. Confirm it is working before launch. Other supplied contact details are included in the page.

The website uses the business story you supplied, including “Established in 1994.” Please verify all business claims and contact details before publishing.

## Add product photos
Put your own photographs in `assets/products/`, for example `kurta-01.jpg`, `suit-01.jpg`, `coord-set-01.jpg`, and `dupatta-01.jpg`. In `index.html`, replace each `.product-placeholder` block with an image element. Example:

```html
<div class="product-image">
  <img src="assets/products/kurta-01.jpg" alt="Chikankari kurta from Shri Purna Chikans">
</div>
```

Add this rule in `styles.css` if it is not already present:

```css
.product-image img { width: 100%; height: 100%; object-fit: cover; display: block; }
```

Use your actual product photos, compressed for fast loading, with descriptive alt text. Do not use unrelated imagery that could misrepresent products.

## Add your logo
Save your logo in `assets/images/` (for example `shri-purna-chikans-logo.png`). To use it in the header and footer, replace the `SPC` monogram span in each `.wordmark` with an image element and add suitable CSS. Keep the original logo file as a backup.

## Free hosting with GitHub Pages
GitHub Pages can host a static website at no hosting charge for eligible public repositories. Domain registration/renewal remains a separate cost. Check GitHub's current official documentation because account features and requirements can change.

1. Sign in or create an account at https://github.com/.
2. Create a **public** repository, e.g. `shri-purna-chikans-website`.
3. Upload the contents of this folder to the repository root. Make sure `index.html`, `styles.css`, `script.js` and `CNAME` are at the root level.
4. Open the repository's **Settings → Pages**. Choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. In the custom domain field, enter `shripurnachikans.com` and save. Keep the `CNAME` file in the repository.
6. At your domain registrar, add the DNS records exactly as shown in GitHub's current custom-domain instructions: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site.
7. **Important for email:** do not remove existing MX, TXT, SPF, DKIM or other mail-related DNS records. Only add/update the website records required by GitHub. Removing mail records can interrupt business email.
8. After DNS has propagated and GitHub verifies the domain, enable **Enforce HTTPS** in Pages settings when available. Test `https://shripurnachikans.com` and `https://www.shripurnachikans.com`.

Official documentation: https://docs.github.com/pages

## Google Search Console
After the site is live, add a Domain property for `shripurnachikans.com` at https://search.google.com/search-console/about and verify it using the TXT record Google provides. Add the TXT record without deleting existing email DNS records. Then use URL Inspection to test the homepage and request indexing. Indexing and ranking are not immediate or guaranteed.

## Final launch checklist
- [ ] Confirm the business email works.
- [ ] Add your logo and actual product photographs.
- [ ] Test phone, WhatsApp, Instagram and map links on a mobile phone.
- [ ] Check the spelling of the business name, address and all claims.
- [ ] Publish on GitHub Pages and connect the custom domain.
- [ ] Preserve email-related DNS records and confirm HTTPS works.
- [ ] Add the live domain to Google Search Console.
