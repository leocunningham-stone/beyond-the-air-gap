# leocunningham.com

A static site for GitHub Pages.

## Structure

```
/
├── index.html              — Entry point
├── selected-works.html     — The corridor
├── bridge.html             — The three questions
├── assets/
│   └── css/
│       └── style.css       — Shared styles
└── essays/
    ├── inversion-point.html
    ├── median-trap.html
    ├── fidelity-gap.html
    ├── averaging-up.html
    ├── when-everything-sounds-true.html
    └── restoration-problem.html
```

## Deployment

1. Create a new GitHub repository named `leocunningham` or configure for your custom domain
2. Push all files to the `main` branch
3. In repository Settings → Pages → set Source to `main` branch, root folder
4. Add your custom domain under Settings → Pages → Custom domain

## Form Handling

The bridge.html contact form currently logs to console only.
To activate form submissions, add a Formspree endpoint:

In bridge.html, replace the form tag with:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Or use Netlify Forms if deploying via Netlify.

## Custom Domain

Add a CNAME file to the root with your domain:
```
leocunningham.com
```
