# renz.writes - Hugo Static Site

This is a Hugo static site generator version of the portfolio website.

## Prerequisites

Install Hugo (Extended version recommended):

**macOS:**
```bash
brew install hugo
```

**Other platforms:**
Visit https://gohugo.io/installation/

## Development

1. **Start the Hugo development server:**
   ```bash
   hugo server
   ```

2. **View your site:**
   Open http://localhost:1313 in your browser

3. **Build for production:**
   ```bash
   hugo
   ```
   This generates static files in the `public/` directory.

## Project Structure

```
├── config.toml          # Hugo configuration
├── content/             # Content files (Markdown)
│   ├── about.md
│   ├── posts.md
│   ├── projects.md
│   └── work.md
├── layouts/             # HTML templates
│   └── _default/
│       ├── baseof.html  # Base template
│       ├── single.html  # Single page template
│       └── posts.html   # Posts page template
├── static/              # Static assets (CSS, images, etc.)
│   └── css/
│       └── custom.css
└── public/              # Generated site (gitignored)
```

## Deployment

### GitHub Pages

1. Build the site:
   ```bash
   hugo
   ```

2. Push the `public/` directory contents to your `gh-pages` branch, or use GitHub Actions to automate this.

### Other Platforms

You can deploy the `public/` directory to any static hosting service:
- Netlify
- Vercel
- Cloudflare Pages
- etc.

## Content Management

- Edit content in `content/*.md` files
- Modify templates in `layouts/` directory
- Update styles in `static/css/custom.css`
- Change site settings in `config.toml`

## Notes

- The original HTML files have been converted to Hugo templates and Markdown content
- Navigation menu is configured in `config.toml`
- All styling is preserved in `static/css/custom.css`

