# 🎯 Advanced Portfolio — Ravi Dongre

A modern, responsive personal portfolio website built with **advanced CSS techniques** including CSS Grid, Flexbox, CSS Variables (custom properties), keyframe animations, and BEM methodology. Features a dark/light theme system, scroll-triggered animations, glassmorphism design, and a mobile-first responsive layout.

---

## 📌 Features

- **CSS Grid Layout** — Complex page layouts using `grid-template-areas`, `auto-fit`, and `minmax()`
- **Flexbox Navigation** — Responsive header with hamburger menu for mobile
- **CSS Variables Theming** — Light/dark mode with `data-theme` attribute and `localStorage` persistence
- **Smooth Animations** — `@keyframes` for hero entrance, scroll-triggered reveal via `IntersectionObserver`
- **Glassmorphism Design** — `backdrop-filter: blur()` on header and cards
- **BEM Methodology** — Organized CSS with Block__Element--Modifier naming
- **Mobile-First Responsive** — Breakpoints at 480px, 768px, and 1024px
- **Advanced Selectors** — `:nth-child()`, `:focus-visible`, `::before`, `::after`, `:not(:placeholder-shown)`
- **Accessibility** — `prefers-reduced-motion` support, `aria-label` attributes, focus indicators

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| HTML5 | Semantic structure |
| CSS3 | Styling, Grid, Flexbox, Animations, Variables |
| JavaScript (ES6) | Theme toggle, mobile nav, scroll animations |
| Google Fonts (Inter) | Modern typography |
| BEM Methodology | CSS organization |

---

## 📂 Project Structure

```
Portfolio-Ravi/
├── index.html              # Main HTML with BEM classes
├── css/
│   ├── main.css            # Design system, variables, BEM components
│   ├── layout.css          # CSS Grid & Flexbox layouts, responsive
│   └── animations.css      # @keyframes, transitions, scroll effects
├── js/
│   └── theme-switcher.js   # Theme toggle, mobile nav, IntersectionObserver
├── Passport_photo.jpeg     # Profile photo
├── README.md               # Documentation (this file)
└── screenshots/            # Visual documentation
```

---

## 🚀 Setup Instructions

### Step 1: Clone the Repository
```bash
git clone https://github.com/ravidongre793/Portfolio-Ravi.git
```

### Step 2: Open in VS Code
Open the project folder in Visual Studio Code.

### Step 3: Run the Project
Open `index.html` in any browser, **OR** use the Live Server extension:
- Right-click on `index.html`
- Select **Open with Live Server**

---

## 🏗️ Advanced CSS Techniques Used

### CSS Grid
- **Page layout**: `grid-template-areas` for header/main/footer structure
- **Skills section**: `repeat(auto-fit, minmax(130px, 1fr))` for responsive grid
- **Projects section**: 1-column → 2-column → 3-column grid across breakpoints
- **About section**: 2-column grid for image + text layout
- **Education timeline**: Grid-based timeline with pseudo-element decorations

### Flexbox
- **Header navigation**: `display: flex` with `justify-content: space-between`
- **Hero content**: Column flex for centered content stacking
- **CTA buttons**: Flex with gap and wrap for button groups
- **Footer socials**: Centered flex layout

### CSS Variables (Custom Properties)
- **Theming**: `:root` (light) and `[data-theme="dark"]` (dark) variable sets
- **Color palette**: Primary, secondary, accent, surface, text, and border colors
- **Spacing system**: `--spacing-xs` through `--spacing-2xl`
- **Transitions**: `--transition-fast`, `--transition-base`, `--transition-slow`
- **Shadows**: `--shadow-sm`, `--shadow-md`, `--shadow-lg`, `--shadow-glow`
- **Glassmorphism**: `--glass-bg`, `--glass-blur`, `--glass-border`

### Animations & Transitions
- **`@keyframes`**: `fadeInUp`, `fadeInLeft`, `scaleIn`, `pulse`, `gradientShift`, `shimmer`
- **Hero entrance**: Staggered animation delays for image → greeting → title → description → CTA
- **Scroll reveal**: `.animate-on-scroll` + `.is-visible` triggered by `IntersectionObserver`
- **Staggered children**: `:nth-child()` delays for skills and project cards
- **Hover effects**: `translateY(-10px)`, `scale(1.05)`, box-shadow transitions

### Advanced Selectors & Pseudo-Elements
- **`::before`**: Gradient top-bar on skill cards, timeline line, section title underline
- **`::after`**: Image overlay on about card, nav link underline animation
- **`:nth-child(n)`**: Staggered animation delays
- **`:focus-visible`**: Accessible focus indicators without affecting click
- **`:not(:placeholder-shown)`**: Floating label behavior on form inputs
- **`:hover`**: Transform and shadow transitions on interactive elements

### BEM Methodology
All classes follow `block__element--modifier` convention:
```
.header__nav-link--active
.hero__title-highlight
.project__card
.skill__icon
.contact__input
.btn--primary
.btn--outline
```

---

## 📋 Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | **Header** | Sticky glassmorphism navbar with logo, nav links, theme toggle, hamburger |
| 2 | **Hero** | Full-viewport intro with animated gradient, profile image, CTA buttons |
| 3 | **About** | Two-column grid with image, bio text, and stats |
| 4 | **Skills** | Auto-fit grid of 15 skill cards with hover effects |
| 5 | **Projects** | Responsive grid of project cards with overlay and tags |
| 6 | **Education** | Timeline layout with pseudo-element decorations |
| 7 | **Contact** | Glassmorphism form with floating labels |
| 8 | **Footer** | Social links with gradient top border |

---

## ⚡ Performance Optimizations

- **`prefers-reduced-motion`** — Disables animations for users who prefer reduced motion
- **Font preconnect** — `<link rel="preconnect">` for Google Fonts
- **Passive scroll listeners** — `{ passive: true }` on scroll events
- **IntersectionObserver** — Efficient scroll detection (no `scroll` event for animations)
- **`will-change`** avoided — Prevents unnecessary GPU layer promotion
- **CSS containment** — Transitions scoped to specific properties

---

## 📸 Screenshots

### Desktop View — Light Theme
*(See screenshots/desktop-light.png)*

### Desktop View — Dark Theme
*(See screenshots/desktop-dark.png)*

### Mobile View
*(See screenshots/mobile.png)*

---

## ✅ Quality Standards Checklist

- [x] CSS Grid for main layout
- [x] CSS Variables for color scheme (light + dark)
- [x] Smooth animations and transitions
- [x] Mobile-first responsive design
- [x] Advanced CSS selectors (`:nth-child`, `:focus-visible`, `::before`, `::after`)
- [x] BEM methodology for CSS
- [x] Semantic HTML5 structure
- [x] Accessible navigation and form
- [x] Cross-browser compatible
- [x] Clean, organized code structure

---

## 👨‍💻 Author

**Ravi Dongre**
Frontend Developer & Web Development Learner
B.Tech IT — MITS Gwalior
