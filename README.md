# Newtons Ecosystem Blog - Static Version

A beautiful, fully-responsive static website for the Newtons Ecosystem (Newtons AI, Newtons HMS, and Newtons Hospitals) with blog, contact form, newsletter, and social media calendar.

## Features

- **Elegant Homepage** with brand showcase for all three Newtons brands
- **Blog System** with 3 pre-published articles (one per brand)
- **Blog Listing Page** with category filtering
- **Individual Blog Posts** with full SEO optimization
- **Contact Form** with three inquiry types (franchise, HMS demo, AI trial)
- **Newsletter Subscription** page
- **Social Media Calendar** with platform and brand filtering
- **Full SEO Optimization** including:
  - Meta tags and descriptions
  - Open Graph tags for social sharing
  - JSON-LD structured data
  - XML sitemap
  - robots.txt
  - Canonical URLs

## File Structure

```
newtons-blog-static/
├── index.html                          # Homepage
├── blog.html                           # Blog listing page
├── contact.html                        # Contact form
├── newsletter.html                     # Newsletter subscription
├── social-calendar.html                # Social media calendar
├── blog/
│   ├── ai-diagnostics-medical-imaging.html
│   ├── autonomous-hospital-management.html
│   └── ai-powered-patient-care.html
├── sitemap.xml                         # XML sitemap for SEO
├── robots.txt                          # Robots file for search engines
├── .gitignore                          # Git ignore file
└── README.md                           # This file
```

## Deployment to GitHub Pages

### Step 1: Create a GitHub Account
If you don't have one, sign up at [github.com](https://github.com)

### Step 2: Create a New Repository
1. Go to [github.com/new](https://github.com/new)
2. Repository name: `newtons-blog-static`
3. Description: "Newtons Ecosystem Blog - Static Version"
4. Make it **Public**
5. Click "Create repository"

### Step 3: Push Code to GitHub

```bash
cd /home/ubuntu/newtons-blog-static

# Configure git
git config user.name "Your Name"
git config user.email "your-email@example.com"

# Add all files
git add .

# Commit
git commit -m "Initial commit: Newtons Ecosystem Blog static version"

# Add remote
git remote add origin https://github.com/YOUR-USERNAME/newtons-blog-static.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Scroll down to **Pages** section
4. Under "Source", select **main** branch
5. Click **Save**
6. Wait 1-2 minutes for deployment
7. Your site will be live at: `https://YOUR-USERNAME.github.io/newtons-blog-static/`

### Step 5: Update URLs

Replace `yourusername` with your actual GitHub username in:
- `index.html` - lines with `og:url` and `canonicalUrl`
- `blog.html` - line with `canonicalUrl`
- All blog post files in `blog/` folder
- `contact.html`, `newsletter.html`, `social-calendar.html`
- `sitemap.xml`

## Local Testing

To test the site locally before deploying:

```bash
# Using Python 3
cd /home/ubuntu/newtons-blog-static
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Customization

### Update Brand Information
Edit the brand descriptions in `index.html` to match your specific offerings.

### Add More Blog Posts
1. Create a new HTML file in the `blog/` folder
2. Copy the structure from existing posts
3. Update the content, metadata, and links
4. Add the post to `blog.html` listing
5. Update `sitemap.xml`

### Modify Colors and Styling
All CSS is embedded in each HTML file. Look for `<style>` tags to customize:
- Brand colors (Newtons AI: blue, HMS: green, Hospitals: red)
- Fonts and typography
- Spacing and layout

### Update Social Media Links
Search for social media URLs and update with your actual profiles.

## SEO Optimization

The site includes:
- ✅ Meta descriptions on all pages
- ✅ Open Graph tags for social sharing
- ✅ JSON-LD structured data for blog posts
- ✅ XML sitemap for search engines
- ✅ robots.txt file
- ✅ Canonical URLs to prevent duplicate content
- ✅ Mobile-responsive design
- ✅ Fast loading times (static HTML)

## Performance

- **Page Load Speed**: Excellent (static HTML, no server required)
- **SEO Score**: Optimized for search engines
- **Mobile Friendly**: Fully responsive design
- **Accessibility**: Semantic HTML and ARIA labels

## Support

For questions or issues:
1. Check the GitHub repository issues
2. Review the HTML comments in the code
3. Ensure all URLs are updated with your GitHub username

## License

© 2026 Newtons Ecosystem. All rights reserved.

---

**Ready to go live?** Follow the deployment steps above to publish your site on GitHub Pages!
