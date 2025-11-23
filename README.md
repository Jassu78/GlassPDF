# GlassPDF Suite

<div align="center">

![GlassPDF Suite](https://img.shields.io/badge/GlassPDF-Suite-blue?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)
![Version](https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge)

**A beautiful, privacy-first PDF manipulation suite with glassmorphism design**

[Features](#-features) • [Tech Stack](#-tech-stack) • [Getting Started](#-getting-started) • [Usage](#-usage) • [Privacy](#-privacy)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Usage](#-usage)
- [Tools Available](#-tools-available)
- [Privacy & Security](#-privacy--security)
- [Browser Support](#-browser-support)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Overview

GlassPDF Suite is a modern, client-side web application for PDF manipulation with a stunning glassmorphism UI inspired by macOS design principles. All processing happens entirely in your browser, ensuring complete privacy and security of your documents.

### Key Highlights

- ✨ **Beautiful UI**: Modern glassmorphism design with smooth animations
- 🔒 **Privacy First**: All processing happens client-side - your files never leave your device
- 📱 **Fully Responsive**: Optimized for mobile, tablet, and desktop
- ⚡ **Fast & Efficient**: No server uploads, instant processing
- 🎨 **Intuitive UX**: Drag-and-drop interface with visual feedback

---

## ✨ Features

### Core Functionality

- **Merge PDFs**: Combine multiple PDF documents into a single file
- **Split PDF**: Extract individual pages from a PDF document
- **Image to PDF**: Convert PNG/JPG images to PDF with drag-and-drop reordering
- **PDF to Image**: Convert PDF pages to high-quality PNG images
- **Compress PDF**: Optimize PDF file size locally
- **Word to PDF**: Convert Microsoft Word documents to PDF (requires server)
- **PPT to PDF**: Convert PowerPoint presentations to PDF (requires server)

### User Experience

- 🖱️ **Drag & Drop**: Intuitive file upload with visual feedback
- 📱 **Touch Support**: Full mobile gesture support for image reordering
- 🎯 **Smart File Handling**: Automatic file type validation
- 🔔 **Toast Notifications**: Real-time feedback for all operations
- 🎨 **Visual Previews**: Image thumbnails with drag-to-reorder functionality
- 📊 **File Status**: Real-time file count and processing status

---

## 🛠️ Tech Stack

### Frontend Technologies

| Category | Technology | Purpose |
|----------|-----------|---------|
| **Markup** | HTML5 | Structure and semantic markup |
| **Styling** | CSS3 | Custom glassmorphism effects, animations |
| **Framework** | Tailwind CSS | Utility-first CSS framework (CDN) |
| **Icons** | Lucide Icons | Modern icon library |
| **Language** | Vanilla JavaScript | Core application logic |

### PDF Processing Libraries

| Library | Version | Purpose |
|---------|---------|---------|
| **pdf-lib** | 1.17.1 | PDF creation, merging, splitting, compression |
| **PDF.js** | 3.11.174 | PDF rendering and page extraction |
| **JSZip** | 3.10.1 | Creating ZIP archives for batch downloads |
| **FileSaver.js** | 2.0.5 | Client-side file downloads |

### Design & UI

- **Glassmorphism**: Custom CSS with backdrop-filter effects
- **Responsive Design**: Mobile-first approach with breakpoints
- **Animations**: CSS transitions and keyframe animations
- **Custom Scrollbars**: Styled scrollbars for better aesthetics

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or build process required!

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/jassu78/GlassPDF.git
   cd GlassPDF
   ```

2. **Open the application**
   - Simply open `index.html` in your web browser
   - Or serve it using a local web server:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     
     # Using PHP
     php -S localhost:8000
     ```

3. **Access the application**
   - Navigate to `http://localhost:8000` (or your chosen port)
   - Start using GlassPDF Suite!

### No Build Process Required

This is a pure client-side application with no dependencies to install. All libraries are loaded via CDN, making it ready to use immediately.

---

## 📖 Usage

### Basic Workflow

1. **Select a Tool**: Choose from the sidebar (desktop) or bottom navigation (mobile)
2. **Upload Files**: 
   - Click the upload area, or
   - Drag and drop files onto the upload zone
3. **Review Files**: Check the file list/preview area
4. **Process**: Click the action button to process your files
5. **Download**: Files are automatically downloaded when processing completes

### Tool-Specific Instructions

#### Merge PDFs
- Upload multiple PDF files
- Files are merged in the order they appear
- Click "Merge Files" to combine them

#### Split PDF
- Upload a single PDF file
- Each page is extracted as a separate PDF
- Download as a ZIP file containing all pages

#### Image to PDF
- Upload multiple images (PNG, JPG, JPEG)
- Drag images to reorder them
- Click "Create PDF" to generate a PDF with images in order

#### PDF to Image
- Upload a single PDF file
- Each page is converted to a PNG image
- Download as a ZIP file containing all images

#### Compress PDF
- Upload a single PDF file
- Click "Optimize PDF" to compress
- Original file is optimized and downloaded

---

## 🛠️ Tools Available

| Tool | Input | Output | Multiple Files |
|------|-------|--------|----------------|
| **Merge PDF** | PDF files | Single PDF | ✅ Yes |
| **Split PDF** | PDF file | ZIP of PDFs | ❌ No |
| **Image to PDF** | Images (PNG/JPG) | Single PDF | ✅ Yes |
| **PDF to Image** | PDF file | ZIP of PNGs | ❌ No |
| **Compress PDF** | PDF file | Optimized PDF | ❌ No |
| **Word to PDF** | DOC/DOCX | PDF | ❌ No* |
| **PPT to PDF** | PPT/PPTX | PDF | ❌ No* |

*Note: Office document conversion requires server-side processing and is currently a placeholder for demonstration.*

---

## 🔒 Privacy & Security

### Client-Side Processing

GlassPDF Suite processes all files entirely in your browser using JavaScript. This means:

- ✅ **No Server Uploads**: Your files never leave your device
- ✅ **No Data Collection**: No tracking, analytics, or data storage
- ✅ **Complete Privacy**: Your documents remain completely private
- ✅ **No Internet Required**: Works offline after initial page load (CDN resources)

### Security Features

- File validation before processing
- Memory-efficient processing
- Automatic cleanup of temporary objects
- No external API calls for core features

---

## 🌐 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |
| Opera | 76+ | ✅ Fully Supported |

### Required Features

- ES6+ JavaScript support
- File API support
- Blob API support
- Canvas API (for PDF to Image)
- Backdrop-filter CSS support (for glassmorphism)

---

## 📁 Project Structure

```
GlassPDF/
│
├── index.html          # Main application file (single-page app)
├── LICENSE             # MIT License
└── README.md           # This file
```

### Architecture

This is a **single-file application** where all HTML, CSS, and JavaScript are contained in `index.html`. This design choice:

- Simplifies deployment
- Eliminates build complexity
- Ensures easy portability
- Reduces maintenance overhead

---

## 🎨 Design Philosophy

### Glassmorphism

The UI uses glassmorphism design principles:

- **Translucent backgrounds** with backdrop blur
- **Subtle borders** for depth
- **Layered shadows** for elevation
- **Smooth transitions** for interactions

### Responsive Breakpoints

- **Mobile**: < 640px (single column, bottom navigation)
- **Tablet**: 640px - 1024px (optimized layout)
- **Desktop**: > 1024px (sidebar navigation, full features)

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'Add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### Areas for Contribution

- Additional PDF tools (rotate, watermark, etc.)
- Performance optimizations
- Accessibility improvements
- UI/UX enhancements
- Bug fixes and documentation

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Jaswanth

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 🙏 Acknowledgments

- **pdf-lib** - Powerful PDF manipulation library
- **PDF.js** - Mozilla's PDF rendering engine
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide Icons** - Beautiful icon library
- **Unsplash** - Background image source

---

## 📧 Contact & Support

- **Issues**: [GitHub Issues](https://github.com/jassu78/GlassPDF/issues)
- **Discussions**: [GitHub Discussions](https://github.com/jassu78/GlassPDF/discussions)


## 🏷️ Tags

`pdf-tools` `pdf-manipulation` `pdf-merge` `pdf-split` `image-to-pdf` `pdf-to-image` `pdf-compress` `glassmorphism` `client-side` `privacy-first` `vanilla-javascript` `tailwindcss` `pdf-lib` `pdfjs` `no-build` `single-page-app` `responsive-design` `drag-and-drop` `file-processing` `web-app` `html5` `css3` `javascript` `browser-based` `offline-capable` `modern-ui` `macos-design`

