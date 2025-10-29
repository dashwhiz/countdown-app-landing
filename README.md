# Countdown App - Landing Page

Minimal landing page for the Countdown App with privacy policy and terms of service.

## Live Site

Once deployed to GitHub Pages:
- **Landing:** https://dashwhiz.github.io/countdown-app-landing/
- **Privacy:** https://dashwhiz.github.io/countdown-app-landing/privacy.html
- **Terms:** https://dashwhiz.github.io/countdown-app-landing/terms.html

## Files

- `index.html` - Main landing page
- `privacy.html` - Privacy policy (required for App Store/Play Store)
- `terms.html` - Terms of service
- `style.css` - Shared styles (dark theme with purple accent: #6750A4)

## Deployment

### GitHub Pages Setup

1. Go to repo Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` / `(root)`
4. Save

Your site will be live at: `https://dashwhiz.github.io/countdown-app-landing/`

### Updating Content

1. Edit HTML files locally
2. Commit and push:
   ```bash
   git add .
   git commit -m "update: your changes"
   git push origin main
   ```
3. GitHub Pages will auto-deploy (takes 1-2 minutes)

## Usage in App

The app menu links to these pages via webview:
- Privacy Policy button → `/privacy.html`
- Help & Support button → `/index.html` (or contact email)
- About button → `/index.html`

URLs should be updated in `lib/app/app_strings.dart`:
```dart
static const String privacyPolicyUrl = 'https://dashwhiz.github.io/countdown-app-landing/privacy.html';
static const String termsOfServiceUrl = 'https://dashwhiz.github.io/countdown-app-landing/terms.html';
```

## Design

- **Dark theme** matching app colors
- **Minimal** design - no JavaScript, no analytics, no tracking
- **Responsive** for mobile and desktop
- **Fast** - simple HTML/CSS only

## License

© 2025 dashwhiz. All rights reserved.
