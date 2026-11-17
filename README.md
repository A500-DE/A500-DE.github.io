# 🚀 Arjun Gupta - Developer Portfolio (GitHub Pages Ready)

Yeh ek modern, responsive aur lightweight developer portfolio website hai jo **GitHub Pages** pe direct host aur render hone ke liye ready banayi gayi hai.

Isme koi bhi complex build tool (npm / webpack wagera) ki zaroorat nahi hai. Pure **HTML5, CSS3, aur JavaScript** me design ki gayi hai jisse GitHub Pages isko instantly 100% render karega.

---

## 📁 File Structure
```text
portfolio/
├── index.html              <-- Main webpage (Semantic, SEO-friendly, fully structured)
├── css/
│   └── style.css           <-- Modern dark/light theme, glassmorphism, responsive grid
├── js/
│   └── script.js           <-- Typing effect, theme toggle, project filter, copy email toast
├── profile-readme/
│   └── README.md           <-- GitHub Profile README template (for github.com/A500-DE profile)
└── README.md               <-- Yeh guide
```

---

## ⚡ 1. Local Laptop Pe Test / Preview Kaise Karein

Aap is portfolio ko 2 aasan tareeko se dekh sakte hain:

### Option A: Direct Open (Sabse Aasan)
- `portfolio` folder me jayein.
- `index.html` file pe **Double Click** karein. Yeh aapke browser (Chrome, Edge, Brave, etc.) me open ho jayegi!

### Option B: VS Code Live Server
- VS Code me `portfolio` folder open karein.
- `index.html` pe right click karein aur **"Open with Live Server"** choose karein.

---

## 🌐 2. GitHub Pages Pe Free Me Live Kaise Karein (Render on GitHub)

GitHub Pages pe render karne ke **2 simple tareeqe** hain:

### Tareeqa 1: Aapka Primary Domain (`https://a500-de.github.io/`) [Recommended]
1. GitHub (`https://github.com`) pe login karein.
2. New Repository banayein jiska naam exact yeh rakhein:  
   **`A500-DE.github.io`**
3. Is repository ko **Public** rakhein.
4. `portfolio` folder ke andar ki sabhi files (`index.html`, `css` folder, `js` folder) ko is repo me push ya upload kar dein.
5. GitHub automatically isko **`https://a500-de.github.io/`** pe live render kar dega! (1-2 minute lag sakta hai).

### Tareeqa 2: Kisi Bhi Normal Repo Me (`https://a500-de.github.io/portfolio/`)
1. GitHub pe ek nayi repo banayein, e.g. `portfolio` ya `my-portfolio`.
2. Saari files push karein:
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git branch -M main
   git remote add origin https://github.com/A500-DE/portfolio.git
   git push -u origin main
   ```
3. GitHub repository page pe jaakar:
   - **Settings** tab pe click karein.
   - Left sidebar me **Pages** pe click karein.
   - **Branch** me `main` select karein aur `/ (root)` chunein, fir **Save** dabayein.
4. Kuch hi seconds me aapko live link mil jayega:  
   `https://a500-de.github.io/portfolio/`

---

## ✏️ 3. Baad Me Nayi Chize Kaise Add Karein (How to Update)

Maine code me bohot saaf aur descriptive comments likhe hain taaki aap asani se nayi chize add kar sakein:

### Naya Project Add Karna:
`index.html` me `<div class="projects-grid">` dhundein (Line ~300 ke aas paas). Kisi ek `project-card` ko copy karein aur paste karke details change kar dein:
```html
<div class="project-card" data-category="fullstack">
  <div class="project-card-header">
    <span class="project-type-tag">Full-Stack / Python</span>
    <span class="project-status"><i class="fa-solid fa-circle-check"></i> Completed</span>
  </div>
  <h3 class="project-title">PROJECT_NAME</h3>
  <h4 class="project-subtitle">Short Tagline</h4>
  <p class="project-description">Description of what it does...</p>
  <ul class="project-features">
    <li><i class="fa-solid fa-circle-check"></i> Feature 1</li>
    <li><i class="fa-solid fa-circle-check"></i> Feature 2</li>
  </ul>
  <div class="project-tech-stack">
    <span class="tech-tag">Python</span>
    <span class="tech-tag">JavaScript</span>
  </div>
  <div class="project-actions">
    <a href="YOUR_GITHUB_REPO_URL" target="_blank" class="project-link-btn">
      <i class="fa-brands fa-github"></i> Repository
    </a>
  </div>
</div>
```

### Nayi Skill Add Karna:
`index.html` me `id="skills"` section me jayein. Relevant category (Programming / Web / Data / Tools) ke andar naya `skill-item` add karein:
```html
<div class="skill-item">
  <div class="skill-top">
    <span class="skill-name-wrap"><i class="fa-solid fa-bolt"></i> Skill Name</span>
    <span class="skill-badge core">Practiced</span> <!-- Options: core, learning, upcoming -->
  </div>
  <p class="skill-notes">Aapne isme kya kiya hai uski short line.</p>
</div>
```

### Roadmap Update Karna:
Jab aap koi naya topic complete kar lein (e.g. JavaScript):
- `class="roadmap-item upcoming"` ko badal kar `class="roadmap-item completed"` kar dein.
- Icon me `<i class="fa-solid fa-check"></i>` laga dein.

---

## 🌟 4. GitHub Profile README (Bonus)
Aapke GitHub account (`github.com/A500-DE`) ke main profile page par bhi aapka bio render ho sake, iske liye maine `portfolio/profile-readme/README.md` file banayi hai.
- GitHub par ek nayi repository banayein jiska naam ho: `A500-DE` (exact aapka username).
- Is repository me `profile-readme/README.md` ka code daal dein.
- GitHub automatically aapke profile page pe ek attractive overview card render karega!

---

💡 **DevFolio CMS note**: Aapka purana `DevFolio-CMS` folder jaisa tha bilkul vaisa hi safe hai aur usme koi changes nahi kiye gaye hain.
