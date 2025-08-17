# BurgTV Portal (Secure via API)

- Calls POST https://api.burgtv.com/api/register_public
- Uses hCaptcha (test sitekey embedded). Replace with your production sitekey:

  In index.html:
    data-sitekey="YOUR_HCAPTCHA_SITEKEY"

## Deployment (Vercel)
- Project: `burgtv-portal-secure`
- Framework: Other (static)
- Build command: none
- Output dir: /
- Domain: app.burgtv.com → point CNAME to Vercel

Make sure the API project has CORS ALLOWED_ORIGIN=https://app.burgtv.com
