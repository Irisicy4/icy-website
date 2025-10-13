# Bingyang (Icy) Wang - Personal Website

A clean, minimal personal website built with Hugo, inspired by Kent C. Dodds' design philosophy but optimized for simplicity and GitHub Pages deployment.

## Features

- **Light Theme**: Clean, professional design inspired by Kent C. Dodds' website
- **Responsive**: Mobile-friendly design
- **Fast Loading**: Static site generation with Hugo
- **Easy Deployment**: Automated GitHub Pages deployment
- **SEO Optimized**: Meta tags and structured data

## Local Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.120.4 or later)
- Git

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   cd YOUR_REPO_NAME
   ```

2. Start the development server:
   ```bash
   hugo server -D
   ```

3. Open your browser to `http://localhost:1313`

### Making Changes

- Edit content in the `content/` directory
- Modify site configuration in `hugo.yaml`
- Customize styling in `assets/scss/custom/_light-theme.scss`
- Add images to `static/img/`

## Deployment Setup

### GitHub Pages Deployment

1. **Create a new GitHub repository** for your website
2. **Push this code** to your repository
3. **Enable GitHub Pages**:
   - Go to repository Settings > Pages
   - Source: "GitHub Actions"
4. **Update configuration**:
   - Edit `hugo.yaml` and update the `baseurl` with your GitHub Pages URL
   - Format: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
5. **Push changes** - the site will automatically deploy

### First-Time Setup Steps

1. **Update Personal Information**:
   - Edit `hugo.yaml`:
     - Change `baseurl` to your GitHub Pages URL
     - Update `title` and `copyright`
     - Update social media links in the `menu.social` section
   
2. **Update Content**:
   - Edit `content/_index.md` with your information
   - Update `content/links.md` with your links
   - Update `content/publications.md` with your publications
   
3. **Add Your Photo**:
   - Replace `static/img/avatar.jpg` with your photo
   - Recommended size: 400x400px, square format

4. **Customize Domain** (Optional):
   - Add a `static/CNAME` file with your custom domain
   - Configure DNS with your domain provider

## File Structure

```
├── .github/workflows/hugo.yml    # GitHub Actions deployment
├── assets/scss/custom/           # Custom styling
├── content/                      # Site content
│   ├── _index.md                # Homepage
│   ├── links.md                 # Links page
│   └── publications.md          # Publications page
├── static/img/                   # Images and assets
├── themes/hugo-theme-stack/      # Hugo theme
└── hugo.yaml                     # Site configuration
```

## Customization

### Colors and Styling
Edit `assets/scss/custom/_light-theme.scss` to customize:
- Color scheme
- Typography
- Layout spacing
- Component styling

### Navigation
Edit the `menu` section in `hugo.yaml` to add/remove navigation items.

### Social Links
Update the `menu.social` section in `hugo.yaml` with your social media profiles.

## Support

If you encounter any issues:

1. Check the [Hugo documentation](https://gohugo.io/documentation/)
2. Verify your `hugo.yaml` configuration
3. Check the GitHub Actions logs for deployment issues

## License

This website template is open source. Feel free to use it as a starting point for your own website.
