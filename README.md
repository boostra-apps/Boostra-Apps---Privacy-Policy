# Boostra Apps - Website

Official website for Boostra Apps, featuring our Shopify applications and privacy policies.

## About Boostra Apps

We build complete, affordable Shopify applications with fast support. We're tired of incomplete apps, expensive pricing, and slow customer service - so we're doing it better.

## Website Structure

### Pages

- **Homepage** (`/`) - Introduction to Boostra Apps and our mission
- **Our Apps** (`/apps/`) - Listing of all our Shopify applications
- **Privacy Policies** - Dedicated privacy policy pages for each app:
  - Boostra Scroll To: `/scroll-to/privacy-policy/`

## Local Development

### Prerequisites

- Hugo (will be installed automatically by Netlify during deployment)
- Node.js and npm (for Netlify CLI)

### Running Locally

If you have Hugo installed:

```bash
hugo server -D
```

Visit http://localhost:1313/

Alternatively, using Netlify CLI:

```bash
npm install netlify-cli -g
netlify dev
```

## Deployment

This site is configured for automatic deployment on Netlify.

### Deploy to Netlify

1. **Via Netlify Dashboard:**
   - Connect your GitHub repository
   - Netlify will automatically detect Hugo configuration
   - Deploy!

2. **Via Netlify CLI:**
   ```bash
   netlify deploy --prod
   ```

### Important URLs After Deployment

- Homepage: `https://your-site.netlify.app/`
- Apps page: `https://your-site.netlify.app/apps/`
- Scroll To Privacy Policy: `https://your-site.netlify.app/scroll-to/privacy-policy/`

Don't forget to update the `baseURL` in `config.yaml` with your actual Netlify domain!

## Adding New Apps

To add a new app:

1. Update `content/apps.md` with the new app information
2. Create a new folder under `content/` for the app (e.g., `content/new-app/`)
3. Add the privacy policy: `content/new-app/privacy-policy.md`

## Contact

For questions or support:
- Email: support@boostra-apps.com

## Built With

- [Hugo](https://gohugo.io/) - Static site generator
- [Netlify](https://www.netlify.com/) - Hosting and deployment
