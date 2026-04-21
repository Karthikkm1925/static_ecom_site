# 🛍️ The Collective — Static E-Commerce Website

## 📌 Overview

The Collective is a multi-page static e-commerce website that replicates a real-world online shopping experience.  
It is designed to demonstrate frontend development skills, project structuring, and production-level deployment using GitHub Pages.

<p>
  🌐 <a href="https://karthikkm1925.github.io/static_ecom_site/">Live Demo</a> • 
  📦 <a href="https://github.com/Karthikkm1925/static_ecom_site">Repository</a>
</p>

## ✨ Features

- 🏠 Interactive homepage with category navigation  
- 👕 Multiple product category pages  
- 🛒 Cart and wishlist UI  
- 🔐 Login & signup pages  
- 💳 Checkout flow (Shipping → Payment → Confirmation)  
- 🎨 Clean and reusable UI design  
- ⚡ Fast global delivery via CDN (GitHub Pages)  

## 🧠 What This Project Demonstrates

- Real-world frontend architecture  
- Clean folder organization  
- Understanding of static hosting  
- Strong Git workflow (add → commit → push)  
- Deployment using GitHub Pages (CI/CD concept)  

## 🏗️ Tech Stack

- HTML5 — Structure  
- CSS3 — Styling  
- JavaScript — Interactivity  
- Git — Version Control  
- GitHub Pages — Hosting  

## 📂 Project Structure

```bash
ECOMMPROJECT/
│
├── index.html                # Entry point (redirect)
│
├── HTML/
│   ├── homepage.html
│   ├── men.html
│   ├── women.html
│   ├── kids.html
│   ├── shoes.html
│   ├── beauty.html
│   ├── jewellery.html
│   ├── decor.html
│   ├── home.html
│   ├── cart.html
│   ├── wishlist.html
│   ├── login.html
│   ├── signup.html
│   ├── payment.html
│   ├── shipping.html
│   └── thankyou.html
│
├── CSS/
├── JavaScript/
└── Images/
```

## 🔁 Redirect Strategy

GitHub Pages requires a root `index.html`, so a redirect is used:

### HTML fallback
```html
<meta http-equiv="refresh" content="0; url=HTML/homepage.html">
```

### JavaScript redirect
```javascript
window.location.replace("HTML/homepage.html");
```

✔ Works even if JavaScript is disabled  
✔ Ensures fast navigation  

## 🚀 Deployment (GitHub Pages)

#### Step 1: Push code
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

#### Step 2: Enable Pages
- Go to **Settings → Pages**  
- Select:  
  - Branch: `main`  
  - Folder: `/ (root)`  

#### Step 3: Access
```
https://<username>.github.io/<repository>/
```
## 🔄 Updating the Project

```bash
git add .
git commit -m "update description"
git push origin main
```

✔ Automatic deployment  
✔ No manual steps required  

## 🎯 Challenges & Solutions

### Challenge 1: GitHub Pages requires `index.html` at root  
**Solution:** Implemented redirect to `/HTML/homepage.html`

### Challenge 2: Project had multiple pages inside subfolders  
**Solution:** Maintained structured folder system with a root entry point  

### Challenge 3: Understanding deployment pipeline  
**Solution:** Used GitHub Pages and learned CI/CD basics  

## 📈 Future Improvements

- 🔗 Backend integration (Node.js / Spring Boot)  
- 🗄️ Database (MongoDB / MySQL)  
- 🛍️ Real cart functionality (localStorage / API)  
- 🔍 Search & filters  
- 📱 Improved mobile responsiveness  
- 🌐 Custom domain  

## 🙋‍♂️ Author

<p>
  <a href="https://github.com/Karthikkm1925"><b>Karthik K M</b></a><br><br>
  📦 <a href="https://github.com/Karthikkm1925/static_ecom_site">Project Repository</a>
</p>

## ⭐ Support

If you found this project useful:

- ⭐ Star the repository  
- 🔁 Share it with others  
- 📘 Use it as a learning reference  


## 📌 Final Note

This project reflects a practical understanding of how real-world frontend applications are structured and deployed using industry-standard tools.
