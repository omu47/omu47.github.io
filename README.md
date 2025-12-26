# S Uma Shankar Reddy - Full Stack Developer Portfolio

[![Deploy Portfolio to GitHub Pages](https://github.com/omu47/omu47.github.io/actions/workflows/static.yml/badge.svg)](https://github.com/omu47/omu47.github.io/actions/workflows/static.yml)

A modern, responsive portfolio website showcasing full-stack development projects, skills, and achievements. Built with HTML, CSS (Tailwind CSS), and deployed automatically using GitHub Actions.

## 🚀 Live Demo

Visit the live portfolio at: [https://omu47.github.io](https://omu47.github.io)

## ✨ Features

- **Modern Design**: Clean, professional layout with smooth animations and transitions
- **Responsive**: Fully responsive design that works on all devices
- **SEO Optimized**: Includes meta tags, Open Graph tags, and structured data
- **Fast Loading**: Minimal dependencies for optimal performance
- **Automated Deployment**: GitHub Actions workflow for seamless deployment

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Tailwind CSS via CDN
- **Deployment**: GitHub Actions → GitHub Pages
- **Version Control**: Git & GitHub

## 📋 Sections

1. **Hero**: Eye-catching introduction with call-to-action buttons
2. **About**: Professional summary and key statistics
3. **Skills**: Comprehensive display of technical skills organized by category
4. **Projects**: Featured projects with descriptions and tech stacks
5. **Achievements**: Notable accomplishments and recognition
6. **Contact**: Contact information and social media links

## 🔄 GitHub Actions Deployment

This portfolio uses GitHub Actions for automatic deployment to GitHub Pages. The workflow:

1. Triggers on push to the `main` branch or manual dispatch
2. Checks out the repository
3. Configures GitHub Pages
4. Verifies all necessary files exist
5. Creates `.nojekyll` file if needed
6. Uploads the site as an artifact
7. Deploys to GitHub Pages

### Workflow Configuration

The deployment workflow is defined in `.github/workflows/static.yml`:

```yaml
name: Deploy Portfolio to GitHub Pages

on:
  push:
    branches: ["main"]
  workflow_dispatch:

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/configure-pages@v5
      - uses: actions/upload-pages-artifact@v3
      - uses: actions/deploy-pages@v4
```

## 🎨 Customization

To customize this portfolio for your own use:

1. **Update Personal Information**:
   - Edit `index.html` with your name, bio, and contact info
   - Update the avatar URL to your GitHub profile picture
   - Modify social media links

2. **Add Your Projects**:
   - Replace project cards with your own projects
   - Update project descriptions and tech stacks
   - Add links to your repositories

3. **Customize Colors**:
   - The portfolio uses a purple-blue gradient theme
   - Edit the Tailwind CSS classes to change colors
   - Modify the gradient classes in hero and section headers

4. **Update Skills**:
   - Add or remove skills in the skills section
   - Organize by your own categories
   - Update emojis and labels

## 📦 Deployment

### Prerequisites

- GitHub account
- Repository named `<username>.github.io`
- GitHub Pages enabled in repository settings

### Steps

1. Fork or clone this repository
2. Enable GitHub Pages in Settings → Pages
3. Set source to "GitHub Actions"
4. Push changes to the `main` branch
5. GitHub Actions will automatically deploy your site

### Manual Deployment

You can also trigger deployment manually:

1. Go to Actions tab in your repository
2. Select "Deploy Portfolio to GitHub Pages"
3. Click "Run workflow"

## 🔧 Development

### Local Development

To run locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/omu47/omu47.github.io.git
   cd omu47.github.io
   ```

2. Open `index.html` in your browser:
   ```bash
   # On macOS
   open index.html
   
   # On Linux
   xdg-open index.html
   
   # Or use a local server
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000` in your browser

### Making Changes

1. Edit `index.html` with your changes
2. Test locally in your browser
3. Commit and push to trigger automatic deployment:
   ```bash
   git add .
   git commit -m "Update portfolio content"
   git push origin main
   ```

## 📚 Inspiration

This portfolio was inspired by successful full-stack developer portfolios:

- [mldangelo/personal-site](https://github.com/mldangelo/personal-site) - Next.js portfolio with GitHub Actions
- [hovinhthanh7893/portfolio](https://github.com/hovinhthanh7893/portfolio) - Clean HTML/CSS/JS portfolio
- [Lucas-Angelo/portfolio](https://github.com/Lucas-Angelo/portfolio) - Minimalist developer portfolio
- [said7388/github-portfolio](https://github.com/said7388/github-portfolio) - GitHub-based portfolio template

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/omu47/omu47.github.io/issues).

## 📧 Contact

- **Email**: umeshreddyumesh420@gmail.com
- **LinkedIn**: [uma-shankar-r](https://www.linkedin.com/in/uma-shankar-r-08a8ab311/)
- **GitHub**: [@omu47](https://github.com/omu47)
- **Itch.io**: [omu47](https://omu47.itch.io)

---

Built with ❤️ by S Uma Shankar Reddy | Deployed with GitHub Actions
