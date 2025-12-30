# Minimalist Crow

A minimalist blog built with 11ty 3.1.2 and entireframework.min.css.

## Features

- **Lightweight CSS Framework** - entireframework at just a few KB
- **Fast Static Site Generation** - 11ty 3.1.2
- **Responsive Design** - Works on all devices
- **Simple & Focused** - Just the essentials

## Quick Start

### Installation

```bash
npm install
```

### Development

```bash
npm start
```

Starts a dev server at `http://localhost:8080` with live reload.

### Build

```bash
npm run build
```

Generates the static site in `_site/`.

## Project Structure

```
minimalist-crow/
├── _includes/       # Layout templates
├── _data/          # Metadata (metadata.json)
├── content/        # Content (markdown)
│   ├── blog/      # Blog posts
│   └── pages/     # Static pages
├── css/           # Stylesheets
├── .eleventy.js   # Eleventy config
└── package.json   # Dependencies
```

## Writing Posts

Create a new markdown file in `content/blog/`:

```markdown
---
layout: post.njk
title: Your Post Title
date: 2024-01-18
tags: [posts, tag-name]
excerpt: "Brief description"
---

Your content here...
```

## Customizing

- Edit `_data/metadata.json` for site metadata
- Modify `css/entireframework.min.css` for styles
- Update `_includes/base.njk` for the main layout
- Edit `_includes/post.njk` for post layout

## License

MIT
