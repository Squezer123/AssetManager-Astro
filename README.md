# 🎯 AssetManager-Astro

A modern web application for managing assets and resources, built with **Astro** and **Tailwind CSS**.

## 📋 Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Available Commands](#available-commands)
- [Technology Stack](#technology-stack)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

- ⚡ **Fast Loading** - Built on Astro with minimal JavaScript
- 🎨 **Modern UI** - Styled with Tailwind CSS
- 📱 **Responsive Design** - Full mobile device support
- 🚀 **Performance Optimized** - Static rendering and SSR
- 🔧 **Easy to Extend** - Modular component architecture
- 🌙 **Dark Mode Ready** - Built with modern design practices

## 📦 Requirements

- **Node.js** version `22.12.0` or higher
- **npm** (comes with Node.js)

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Squezer123/AssetManager-Astro.git
   cd AssetManager-Astro
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure environment variables** (if needed):
   ```bash
   # Create .env.local file
   cp .env.example .env.local
   
   # Edit .env.local with your values
   ```

## 🚀 Getting Started

### Development Server

Start the development server at `localhost:4321`:

```bash
npm run dev
```

The application will be available at: http://localhost:4321

Open the source code and start editing. The page will automatically reload as you make changes.

### Production Build

Build the application for production:

```bash
npm run build
```

The build output will be generated in the `./dist/` directory.

### Preview Build

Preview your production build locally before deployment:

```bash
npm run preview
```

## 📁 Project Structure

```
AssetManager-Astro/
├── public/              # Static files (images, favicon, etc.)
├── src/
│   ├── pages/          # Astro pages (each file = route)
│   │   └── index.astro # Home page
│   ├── components/     # Reusable components
│   ├── layouts/        # Page layouts
│   └── styles/         # Global styles
├── .vscode/            # VS Code configuration
├── package.json        # Dependencies and scripts
├── tsconfig.json       # TypeScript configuration
├── astro.config.mjs    # Astro configuration
└── README.md           # This file
```

### How Routing Works

Astro generates routes based on the file structure in `src/pages/`:
- `src/pages/index.astro` → `/`
- `src/pages/about.astro` → `/about`
- `src/pages/posts/[id].astro` → `/posts/:id` (dynamic routing)
- `src/pages/blog/[...slug].astro` → `/blog/*` (catch-all routes)

## 📌 Available Commands

All commands are run from the root of the project:

| Command | Description |
|---------|-------------|
| `npm run dev` | Start the development server at `localhost:4321` |
| `npm run build` | Build the application to `./dist/` |
| `npm run preview` | Preview the built application locally |
| `npm run astro ...` | Run Astro CLI commands |
| `npm run astro -- --help` | Get help using the Astro CLI |

## 🛠️ Technology Stack

### Frontend
- **[Astro](https://astro.build)** - The web framework for building static and hybrid websites
- **[Tailwind CSS](https://tailwindcss.com)** - Utility-first CSS framework
- **[TypeScript](https://www.typescriptlang.org/)** - JavaScript with syntax for types
- **[@tailwindcss/vite](https://github.com/tailwindlabs/tailwindcss)** - Tailwind CSS Vite plugin

### Tools
- **npm** - Package manager
- **Vite** - Next generation frontend tooling
- **ESM** - ES modules support

### Versions
- Astro: ^7.1.6
- Tailwind CSS: ^4.3.3
- Node.js: >=22.12.0

## 📚 Resources

### Documentation
- [Astro Documentation](https://docs.astro.build) - Complete guide to Astro
- [Astro Guides](https://docs.astro.build/guides) - Step-by-step tutorials
- [Tailwind CSS Documentation](https://tailwindcss.com/docs) - Tailwind CSS reference
- [TypeScript Handbook](https://www.typescriptlang.org/docs/) - TypeScript learning resource

### Community
- [Astro Discord](https://astro.build/chat) - Official Astro Discord server
- [GitHub Discussions](https://github.com/Squezer123/AssetManager-Astro/discussions) - Project discussions
- [Astro Community](https://astro.build/community) - Community resources

## 🤝 Contributing

We welcome contributions! Here's how to get started:

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on GitHub
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. **Make your changes**
   ```bash
   # Edit files and create awesome features
   ```

4. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/AmazingFeature
   ```

6. **Open a Pull Request**
   - Go to the main repository
   - Click "New Pull Request"
   - Select your branch and submit

### Development Guidelines
- Follow the existing code style
- Write meaningful commit messages
- Test your changes locally before submitting
- Keep Pull Requests focused and concise

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**Squezer123**

- GitHub: [@Squezer123](https://github.com/Squezer123)
- Repository: [AssetManager-Astro](https://github.com/Squezer123/AssetManager-Astro)

## 📞 Support

If you encounter any issues:

1. Check [existing issues](https://github.com/Squezer123/AssetManager-Astro/issues)
2. Open a [new issue](https://github.com/Squezer123/AssetManager-Astro/issues/new)
3. Describe the problem and steps to reproduce
4. Join the [Astro Discord](https://astro.build/chat) for community help

## 🎓 Learning Resources

New to Astro? Check out these resources:
- [Astro Crash Course](https://docs.astro.build/en/getting-started/) - Quick start guide
- [Building a Blog](https://docs.astro.build/en/tutorial/0-introduction/) - Interactive tutorial
- [Astro Integration Guide](https://docs.astro.build/en/guides/integrations-guide/) - Add more features

## 🚀 Deployment

### Deploy to Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Deploy to Netlify
```bash
# Build the project
npm run build

# Deploy the dist folder to Netlify
```

### Deploy to Cloudflare Pages
```bash
# Follow Cloudflare Pages documentation
# Connect your GitHub repository
```

## 📈 Performance

This project is optimized for performance:
- **Zero JS by default** - HTML and CSS only, unless needed
- **Partial hydration** - Load interactive components only where needed
- **Image optimization** - Automatic image optimization
- **CSS minification** - Production CSS is minified
- **Code splitting** - Split code automatically for better caching

## 🐛 Troubleshooting

### Port 4321 already in use
```bash
# Kill the process using port 4321, or use a different port
npm run dev -- --port 3000
```

### Node version issues
```bash
# Check your Node version
node --version

# Update to the required version
# Visit https://nodejs.org/ to download Node.js 22.12.0 or higher
```

### Dependencies issues
```bash
# Clear npm cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

---

**Last Updated:** 2026  
**Status:** Active Development  
**Node.js Required:** >=22.12.0  
**Astro Version:** ^7.1.6  
**Tailwind CSS Version:** ^4.3.3

Made with ❤️ by [Squezer123](https://github.com/Squezer123)
