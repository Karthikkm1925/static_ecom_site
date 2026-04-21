# 🚀 The Collective: Deployment & Mobile Optimization Guide

This guide is designed to help you understand how to host your static website for free on GitHub Pages and how we transformed it from a desktop-only site into a fully mobile-responsive experience. You can use this guide to teach others or for your own interview preparation!

---

## 🏗️ PART 1: Deployment & Hosting (GitHub Pages)

### 1. Preparing Your Project
- Ensure your project has an `index.html` file in the **root directory**. This is the entry point for your website.
- Organize your files into logical folders: `/CSS`, `/JavaScript`, `/HTML`, `/Images`.

### 2. Creating a GitHub Repository
1. Log in to [GitHub](https://github.com).
2. Click the **+** (Plus) icon in the top right and select **New repository**.
3. Name your repository (e.g., `ecommerce-website`).
4. Set it to **Public** and click **Create repository**.

### 3. Pushing Your Files to GitHub
Open your terminal (Command Prompt, PowerShell, or Git Bash) in your project folder and run:
```bash
git init
git add .
git commit -m "Initial commit - Static Ecommerce Site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

### 4. Activating GitHub Pages
1. Go to your repository on GitHub.
2. Click **Settings** (top tab).
3. Select **Pages** from the left sidebar.
4. Under **Build and deployment**, select:
   - Branch: `main`
   - Folder: `/(root)`
5. Click **Save**.
6. Wait 1-2 minutes. Your site will be live at: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

---

## 📱 PART 2: Mobile Optimization (Step-by-Step)

We converted the site from desktop-only to mobile-friendly using three main techniques:

### 1. The Viewport Meta Tag
Every HTML file MUST have this inside the `<head>` tag. It tells the browser how to scale the page on mobile devices.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### 2. CSS Media Queries
Media queries allow us to apply different styles based on the screen size (width). 
- **Example**: Stacking elements that were side-by-side on desktop.
```css
/* On screens smaller than 768px... */
@media (max-width: 768px) {
  .container-box {
    flex-direction: column; /* Stack vertically instead of horizontally */
  }
}
```

### 3. The Hamburger Menu
On mobile, the navigation links take up too much space. We replaced them with a "Hamburger" icon (three lines).
- **Structure**:
  - A button (`.mobile-toggle`) that appears only on mobile.
  - A JavaScript listener that toggles a class (e.g., `.active`) to show/hide the menu.

---

## 🛠️ PART 3: Key Files Explained
- **`index.html`**: The main entry point (root).
- **`homepage.html`**: The main landing page with the responsive header and products.
- **`homepage.js`**: Contains the logic to handle the mobile menu toggle.
- **`payment.html` / `shipping.html`**: Optimized to ensure the checkout flow is easy to use on a phone.

---

## 🎓 Tips for Interviews
- **Performance**: Mention that you used Vanilla HTML/CSS for faster load times since there's no heavy framework.
- **Responsive Design**: Explain that "Mobile First" design is an industry standard, and you ensured the site works on any device size.
- **Version Control**: Demonstrate your knowledge of Git by explaining how you used `git add`, `git commit`, and `git push`.

---
*Created by [The Collective Team] for educational purposes.*
