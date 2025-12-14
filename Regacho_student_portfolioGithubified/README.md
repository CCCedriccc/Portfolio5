# Student Portfolio

This is a static portfolio website hosted on GitHub Pages.

## What Changed

- **Converted from Flask app** to static HTML files
- Removed authentication (login/register)
- Created 3 main pages: `index.html` (home), `portfolio.html` (projects), `about.html` (about me)
- All files are pure HTML/CSS with no backend required

## Files Included

- `index.html` - Home page
- `portfolio.html` - Portfolio projects page
- `about.html` - About me page
- `static/site.css` - Styling
- `static/images/` - Your images
- `static/uploads/` - Project images

## How to Customize

### Edit Your Information
1. Open `about.html` and update the bio, course, and skills section
2. Open `portfolio.html` and add your actual projects

### Add Projects
In `portfolio.html`, duplicate a `.project-card` div and update:
```html
<div class="project-card">
    <h3>Your Project Title</h3>
    <img src="static/uploads/your-image.jpg" alt="Project">
    <p><strong>Description:</strong> Describe your project...</p>
    <p><strong>Date:</strong> 2024-12-11</p>
</div>
```

## Deploying to GitHub Pages

1. Push your changes to GitHub:
   ```bash
   git add .
   git commit -m "Convert to static portfolio"
   git push origin main
   ```

2. Go to your repository settings → Pages
3. Select **main** branch as the source
4. Your site will be available at: `https://cccedriccc.github.io/Portfolio3/`

## Local Testing

Open `index.html` in your browser directly, or run:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`

## Notes

- The old Flask app (`app.py`) is no longer needed - you can keep it for reference or delete it
- All functionality now happens in the browser (no database, authentication, or server)
- To add interactivity later, you can use JavaScript

