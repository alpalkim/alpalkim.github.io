# alpalkim.github.io

Personal website for ALP ALKIM

## Pages

- **Privacy Policy**: `/scoreblastprivacypolicy.html` - Privacy policy for Score Blaster app
- **Support/Contact**: `/support.html` - Contact form for support requests and inquiries

## Deployment

This site is designed to be deployed on GitHub Pages with Netlify Forms integration for the contact form.

### Setting up Netlify Forms

To enable the contact form at `/support.html`:

1. Deploy the site to Netlify or configure it with GitHub Pages + Netlify
2. Netlify will automatically detect forms with the `data-netlify="true"` attribute
3. Configure email notifications in your Netlify dashboard:
   - Go to Settings → Forms
   - Add the notification email address (alpalkim@gmail.com)
   - Enable spam filtering and reCAPTCHA

The form includes:
- Spam protection with honeypot field
- reCAPTCHA integration
- Client-side validation
- Mobile-responsive design

