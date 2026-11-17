# CLAUDE.md - AI & Data Science Notes Project Guidelines

## 1. Project Purpose & Core Architecture
- **Project Name**: AI & Data Science Learning Notes
- **Purpose**: Build a scalable personal technical notes website for easy reference on machine learning, deep learning, and RAG-related topics.
- **Tech Stack**: Pure HTML5, Tailwind CSS (via CDN for lightweight setup), Vanilla JavaScript.
- **Deployment**: Static website hosting via GitHub Pages.

## 2. Directory Structure & File Naming Conventions
The project root directory must maintain the following structure:
├── index.html          # Homepage (includes article lists and navigation)
├── CLAUDE.md           # Project guideline document
├── content/            # Directory storing all article contents
│   ├── ml-basics.html  # Machine Learning basics note page
│   └── rag-intro.html  # RAG system architecture note page
└── assets/             # Static resources (images, custom CSS/JS)
├── css/
└── js/

- **File Naming Rule**: All newly created content pages must be placed inside the `content/` folder using lowercase English words separated by hyphens (e.g., `neural-networks.html`).

## 3. Overall Style & Design Guidelines
- **Design Style**: Minimalist, modern technical documentation style (inspired by Tailwind UI / official documentation aesthetics).
- **Color Palette**:
  - Primary: Slate / Indigo (calm technical blue-gray tones).
  - Background: `bg-slate-50` or `bg-white`.
  - Typography Color: `text-slate-800` (headings/body text), `text-slate-500` (secondary text/tags).
- **Layout Requirements**:
  - Must support Responsive Web Design (RWD) for smooth viewing on both mobile devices and desktops.
  - Code snippets must use highlighted blocks (`<pre><code>`) with a light gray background and subtle borders.

## 4. Content Formatting Rules
When the AI assists in creating or modifying an article page, the new page must follow this standard HTML structural skeleton:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Article Title - AI & Data Science Notes</title>
    <script src="[https://cdn.tailwindcss.com](https://cdn.tailwindcss.com)"></script>
</head>
<body class="bg-slate-50 text-slate-800 font-sans leading-relaxed">
    <!-- Navigation Bar -->
    <nav class="bg-white border-b border-slate-200 py-4 px-6 mb-8 shadow-sm">
        <div class="max-w-4xl mx-auto flex justify-between items-center">
            <a href="../index.html" class="font-bold text-indigo-600 hover:text-indigo-800">← Back to Home</a>
            <span class="text-sm text-slate-500">AI Knowledge Base</span>
        </div>
    </nav>

    <!-- Main Content Area -->
    <main class="max-w-4xl mx-auto bg-white p-8 rounded-xl shadow-sm border border-slate-200 mb-12">
        <h1 class="text-3xl font-bold mb-4 text-slate-900">Article Main Title</h1>
        <p class="text-sm text-slate-500 mb-6">Published: YYYY-MM-DD | Category: Technical Notes</p>
        
        <article class="space-y-6">
            <!-- Content paragraphs, headings, and code blocks go here -->
        </article>
    </main>
</body>
</html>