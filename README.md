# EBGS-ONLINE-PAGE
PAGINA APP EPIC 

## Epic Games Domain Verification

This repository hosts the GitHub Pages site for Epic Games domain verification.

### Important Note About TXT DNS Records

Since this site is hosted on GitHub Pages (`gamrabadr.github.io`), you **cannot directly add TXT DNS records** because GitHub controls the DNS for `*.github.io` subdomains.

### Alternative Verification Methods

For Epic Games verification on GitHub Pages, use **file-based verification**:

1. **Verification File**: Place the Epic verification content in `.well-known/epic-domain-verification.txt`
2. **Verification Page**: The `epic-domain.html` page confirms domain ownership

### How to Add Your Epic Domain Secret

1. Get your domain secret from the Epic Developer Portal
2. Replace the placeholder content in `.well-known/epic-domain-verification.txt` with your actual secret
3. Commit and push the changes
4. Wait for GitHub Pages deployment to complete
5. Click "Verify" in the Epic Developer Portal

### Using a Custom Domain (For TXT DNS Verification)

If you need to add a TXT DNS record for Epic verification:

1. Register a custom domain (e.g., `ebgs-online.com`)
2. Configure it as a custom domain for this GitHub Pages site
3. Add the TXT record through your domain registrar's DNS settings
4. The TXT record format is typically: `epic-domain-verification=YOUR_SECRET_HERE`

### Files Structure

- `index.html` - Main page
- `epic-domain.html` - Epic verification information page
- `epic-verification.html` - Additional verification page
- `.well-known/epic-domain-verification.txt` - Epic verification file
- `privacy.html` - Privacy policy
