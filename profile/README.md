# Lito Docs

> Beautiful documentation sites from Markdown. Fast, simple, and open-source.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

## 🌟 Overview

Lito Docs is an organization building powerful tools to help you create beautiful, SEO-optimized documentation sites from Markdown and MDX files. With support for multiple frameworks, AI-powered content generation, and zero-config setup, Lito makes documentation easy and enjoyable.

## 📦 Repositories

### Core Tools

#### [@litodocs/cli](https://github.com/Lito-docs/lito)
The main CLI tool for building and serving documentation sites.

**Features:**
- 🚀 Multi-framework support (Astro, Next.js, Nuxt, React, Vue)
- 📝 Markdown & MDX with frontmatter
- 🎨 Dynamic theming with OKLCH color generation
- 🌍 i18n support for 40+ languages
- 📚 Built-in versioning system
- ⚡ Hot reload and fast builds
- 🎯 SEO optimized

**Quick Start:**
```bash
npm install -g @litodocs/cli
lito init
lito dev -i ./my-docs
```

#### [@lito/generate](https://github.com/Lito-docs/lito-generate)
AI-powered documentation generator that analyzes codebases and generates comprehensive documentation.

**Features:**
- 🤖 Multi-provider LLM support (OpenAI, Claude, Gemini, Ollama)
- 🔧 Agentic architecture with specialized agents
- 🎯 SEO optimization with structured data
- 📊 Sitemap and meta tag generation
- 🔄 Lito-compatible output format

**Quick Start:**
```bash
npm install -g @lito/generate
lito-generate generate -i ./my-project -p openai
```

### Official Templates

#### [lito-astro-template](https://github.com/Lito-docs/lito-astro-template)
**Default template** - Blazing-fast static documentation site built with Astro.

- ⚡ Fastest build times
- 🎯 Optimal for static content
- 💼 Production-ready components
- 📦 Zero JavaScript by default

**Usage:**
```bash
lito dev -i ./docs --template astro
```

#### [lito-next-template](https://github.com/Lito-docs/lito-next-template)
Next.js template with React ecosystem support and SSR capabilities.

- ⚛️ Full React support
- 🔄 Server-side rendering
- 🎨 Modern UI components
- 📱 Responsive design

**Usage:**
```bash
lito dev -i ./docs --template next
```

#### [lito-nuxt-template](https://github.com/Lito-docs/lito-nuxt-template)
Nuxt template for Vue developers with SSR/SSG support.

- 🖖 Vue 3 ecosystem
- 🔄 Universal rendering
- 🎨 Nuxt Content integration
- 📦 Auto-imports

**Usage:**
```bash
lito dev -i ./docs --template nuxt
```

### Examples

#### [sample-docs](https://github.com/Lito-docs/sample-docs)
Comprehensive demo showcasing all Lito features and capabilities.

**Includes:**
- 📚 Multi-language documentation (English, Spanish)
- 🎯 API reference examples
- 📖 Tutorial and guide structures
- 🎨 Custom landing page
- 🖼️ Image and asset management
- 🔧 Advanced configuration examples

## 🚀 Getting Started

### 1. Install the CLI

```bash
npm install -g @litodocs/cli
```

### 2. Initialize Your Project

```bash
lito init
```

### 3. Choose Your Workflow

#### Option A: Manual Documentation
Write your documentation manually in Markdown/MDX files:

```bash
# Start development server
lito dev -i ./my-docs

# Build for production
lito build -i ./my-docs -o ./dist
```

#### Option B: AI-Generated Documentation
Let AI analyze your codebase and generate documentation:

```bash
npm install -g @lito/generate
lito-generate generate -i ./my-project -p openai
```

## 🎯 Key Features

### Multi-Framework Support
Choose the framework that fits your workflow:
- **Astro** - Fast static sites (default)
- **Next.js** - React with SSR/SSG
- **Nuxt** - Vue with SSR/SSG
- **React** - Vite-powered React app
- **Vue** - Vite-powered Vue app

### Template System
```bash
# Use official templates
lito dev -i ./docs --template astro
lito dev -i ./docs --template next
lito dev -i ./docs --template nuxt

# Use custom GitHub templates
lito dev -i ./docs --template github:owner/repo

# Use local templates
lito dev -i ./docs --template ./path/to/template
```

### AI Documentation Generation
```bash
# Analyze and generate documentation
lito-generate generate -i ./my-project -p anthropic

# Multiple LLM providers supported
lito-generate generate -i ./my-project -p openai -m gpt-4o
lito-generate generate -i ./my-project -p google -m gemini-2.0-flash
lito-generate generate -i ./my-project -p ollama -m llama3.2
```

### Built-in Features
- 🎨 **Dynamic Theming** - Generate color palettes from primary colors
- 🌍 **Internationalization** - Support for 40+ languages
- 📚 **Versioning** - Document multiple versions with switcher
- 🔍 **Search** - Built-in search functionality
- 📱 **Responsive** - Mobile-first design
- ♿ **Accessible** - WCAG compliant
- 🎯 **SEO** - Optimized meta tags and structure

## 📚 Documentation Structure

Lito uses a simple folder-based structure:

```
my-docs/
├── docs-config.json          # Configuration file
├── introduction/
│   ├── getting-started.mdx
│   └── installation.mdx
├── guides/
│   ├── basic-usage.mdx
│   └── advanced-features.mdx
├── api/
│   └── reference.mdx
├── _landing/                 # Custom landing page (optional)
│   ├── index.html
│   ├── styles.css
│   └── script.js
└── _assets/                  # Static assets
    └── logo.svg
```

## 🛠️ CLI Commands

### Lito CLI
```bash
lito init            # Initialize new project
lito dev            # Start dev server
lito build          # Build for production
lito preview        # Preview production build
lito validate       # Validate configuration
lito doctor         # Diagnose issues
lito info           # Show project info
lito eject          # Export full source
lito template       # Manage templates
lito upgrade        # Update CLI
```

### Lito Generate
```bash
lito-generate generate   # Generate documentation
lito-generate analyze    # Analyze codebase only
lito-generate init       # Initialize docs project
```

## 🤝 Contributing

We welcome contributions to all Lito projects! Please see individual repositories for contribution guidelines.

### Development Setup

```bash
# Clone the repository
git clone https://github.com/Lito-docs/<repo-name>

# Install dependencies
pnpm install

# Run in development mode
pnpm dev
```

## 📝 License

All Lito projects are open-source and licensed under the [MIT License](LICENSE).

## 🔗 Links

- **Website**: [litodocs.dev](https://litodocs.dev)
- **Documentation**: [docs.litodocs.dev](https://docs.litodocs.dev)
- **GitHub Organization**: [github.com/Lito-docs](https://github.com/Lito-docs)
- **NPM**: [@litodocs/cli](https://www.npmjs.com/package/@litodocs/cli)

## 💬 Support

- 🐛 **Bug Reports**: [Open an issue](https://github.com/Lito-docs/cli/issues)
- 💡 **Feature Requests**: [Submit a request](https://github.com/Lito-docs/cli/issues)
- 📧 **Email**: support@litodocs.dev
- 💬 **Discord**: [Join our community](https://discord.gg/litodocs)

## 🌟 Acknowledgments

Built with love by the Lito Docs team and powered by:
- [Astro](https://astro.build)
- [Next.js](https://nextjs.org)
- [Nuxt](https://nuxt.com)
- [MDX](https://mdxjs.com)

---

<p align="center">
  <strong>Make documentation beautiful again ✨</strong>
</p>
