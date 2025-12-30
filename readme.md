# Beeyo.ai Landing Page

A modern, responsive landing page for Beeyo.ai built with Hugo and Tailwind CSS.

## 🚀 Features

- **Virtual Try-On**: Experience fashion before you buy
- **AI-Powered Styling**: Personalized outfit recommendations
- **Digital Closet**: Smart wardrobe management
- **Fully Responsive**: Optimized for all devices
- **Fast Performance**: Static site generation with Hugo

## 🛠️ Tech Stack

- **[Hugo](https://gohugo.io/)** - Static site generator
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework (via CDN)
- **[Lucide Icons](https://lucide.dev/)** - Beautiful icon library
- **GitHub Pages** - Hosting and deployment

## 📁 Project Structure

```
beeyo-hugo-website/
├── .github/
│   └── workflows/
│       └── hugo.yaml          # GitHub Actions deployment workflow
├── content/
│   └── _index.md              # Homepage content
├── layouts/
│   └── index.html             # Homepage template
├── hugo.toml                  # Hugo configuration
├── .gitignore                 # Git ignore rules
└── README.md                  # This file
```

## 🚦 Getting Started

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.139.0 or later)
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/beeyoai/beeyo-hugo-website.git
   cd beeyo-hugo-website
   ```

2. **Run the development server**
   ```bash
   hugo server -D
   ```

3. **Open your browser**
   Navigate to `http://localhost:1313`

### Building for Production

```bash
hugo --gc --minify
```

The built site will be in the `public/` directory.

## 🌐 Deployment to GitHub Pages

### Setup Instructions

1. **Enable GitHub Pages**
   - Go to your repository settings
   - Navigate to **Pages** section
   - Under **Source**, select **GitHub Actions**

2. **Update baseURL**
   Edit [hugo.toml](hugo.toml) and update the `baseURL`:
   ```toml
   baseURL = "https://beeyoai.github.io/beeyo-hugo-website/"
   ```

3. **Push to main branch**
   ```bash
   git add .
   git commit -m "Initial Hugo site setup"
   git push origin main
   ```

4. **Automatic Deployment**
   The GitHub Actions workflow will automatically:
   - Build your Hugo site
   - Deploy to GitHub Pages
   - Your site will be live at: `https://beeyoai.github.io/beeyo-hugo-website/`

### Manual Deployment

You can also trigger deployment manually from the **Actions** tab in your GitHub repository.

## 🎨 Customization

### Brand Colors

The site uses custom Tailwind colors defined in the `<head>` section of [layouts/index.html](layouts/index.html):

- **Purple**: `#6D28D9` - Primary brand color
- **Lime**: `#CCFF00` - Accent color
- **Dark**: `#0F172A` - Text and backgrounds

### Content Updates

Edit [content/_index.md](content/_index.md) to update meta information and page content.

### Layout Changes

Modify [layouts/index.html](layouts/index.html) to change the page structure and design.

## 📝 License

© 2025 Beeyo. All rights reserved.

## 🤝 Contributing

This is a private project. For any questions or suggestions, please contact the Beeyo.ai team.

---

Made with ❤️ for the 370M Gen Z shoppers of India.
