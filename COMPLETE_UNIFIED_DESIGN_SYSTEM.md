# COMPLETE DESIGN SYSTEM - ALL-IN-ONE REFERENCE

---

## TABLE OF CONTENTS
1. [Color System](#color-system)
2. [Typography](#typography)
3. [Spacing System](#spacing-system)
4. [Motion & Animations](#motion--animations)
5. [Shadow System](#shadow-system)
6. [Border Radius](#border-radius)
7. [Dark/Light Mode Toggle](#darklight-mode-toggle)
8. [Component Styles](#component-styles)
9. [Responsive Breakpoints](#responsive-breakpoints)
10. [CSS Variables Summary](#css-variables-summary)
11. [HTML Template](#html-template)
12. [JavaScript Implementation](#javascript-implementation)

---

## COLOR SYSTEM

### Light Mode - Primary Colors

```css
:root {
  /* Core Brand Colors - Sarvam Inspired */
  --primary-blue-dark: #0F4C75;      /* Darkest - Headings, dark backgrounds */
  --primary-blue: #1F3A93;           /* Main primary color */
  --primary-blue-light: #3B82F6;     /* Light blue - Hover states */
  --primary-blue-lighter: #60A5FA;   /* Even lighter - Disabled, subtle */
  
  /* Orange Accent Colors */
  --accent-orange: #FF6B35;          /* Main accent - CTAs, highlights */
  --accent-orange-light: #FF8C42;    /* Light orange - Hover states */
  --accent-orange-pale: #FFCF9B;     /* Very light - Subtle accents */
  
  /* Secondary & Complementary */
  --secondary-teal: #06B6D4;         /* Teal - Alternative accent */
  --secondary-purple: #8B5CF6;       /* Purple - Secondary actions */
  
  /* Neutral Colors - Light Mode */
  --neutral-white: #FFFFFF;
  --neutral-50: #F9FAFB;
  --neutral-100: #F3F4F6;
  --neutral-200: #E5E7EB;
  --neutral-300: #D1D5DB;
  --neutral-400: #9CA3AF;
  --neutral-500: #6B7280;
  --neutral-600: #4B5563;
  --neutral-700: #1F2937;
  --neutral-800: #111827;
  
  /* Semantic Colors - Light Mode */
  --success: #10B981;
  --success-light: #D1FAE5;
  --warning: #F59E0B;
  --warning-light: #FEF3C7;
  --error: #EF4444;
  --error-light: #FEE2E2;
  --info: #3B82F6;
  --info-light: #DBEAFE;
  
  /* Text Colors - Light Mode */
  --text-primary: #1F2937;
  --text-secondary: #6B7280;
  --text-tertiary: #9CA3AF;
  --text-inverse: #FFFFFF;
  
  /* Background Colors - Light Mode */
  --bg-primary: #FFFFFF;
  --bg-secondary: #F9FAFB;
  --bg-tertiary: #F3F4F6;
  
  /* Border & Shadow - Light Mode */
  --border-color: #E5E7EB;
  --border-light: #F3F4F6;
  --border-dark: #D1D5DB;
  
  /* Gradients - Light Mode */
  --gradient-blue-to-orange: linear-gradient(135deg, #0F4C75 0%, #3B82F6 50%, #FF6B35 100%);
  --gradient-smooth-blue-orange: linear-gradient(90deg, #1F3A93 0%, #2563EB 25%, #FF8C42 75%, #FF6B35 100%);
  --gradient-button: linear-gradient(135deg, #1F3A93 0%, #3B82F6 100%);
  --gradient-accent: linear-gradient(90deg, #FF6B35 0%, #FF8C42 100%);
  --gradient-card: linear-gradient(135deg, rgba(31, 58, 147, 0.05) 0%, rgba(255, 107, 53, 0.05) 100%);
  --gradient-bg: linear-gradient(180deg, #FFFFFF 0%, #F9FAFB 100%);
}
```

### Dark Mode - Primary Colors

```css
html[data-theme="dark"],
@media (prefers-color-scheme: dark) {
  /* Core Brand Colors - Adjusted for Dark Mode */
  --primary-blue-dark: #1E3A8A;
  --primary-blue: #3B82F6;
  --primary-blue-light: #60A5FA;
  --primary-blue-lighter: #93C5FD;
  
  /* Orange Accent Colors - Adjusted for Dark Mode */
  --accent-orange: #FF8C42;
  --accent-orange-light: #FFCF9B;
  --accent-orange-pale: #FFE0CC;
  
  /* Secondary & Complementary */
  --secondary-teal: #0891B2;
  --secondary-purple: #A78BFA;
  
  /* Neutral Colors - Dark Mode */
  --neutral-white: #0F172A;
  --neutral-50: #1E293B;
  --neutral-100: #1F2937;
  --neutral-200: #374151;
  --neutral-300: #4B5563;
  --neutral-400: #6B7280;
  --neutral-500: #9CA3AF;
  --neutral-600: #D1D5DB;
  --neutral-700: #E5E7EB;
  --neutral-800: #F3F4F6;
  
  /* Semantic Colors - Dark Mode */
  --success: #10B981;
  --success-light: #064E3B;
  --warning: #FBBF24;
  --warning-light: #78350F;
  --error: #F87171;
  --error-light: #7F1D1D;
  --info: #60A5FA;
  --info-light: #1E3A8A;
  
  /* Text Colors - Dark Mode */
  --text-primary: #F3F4F6;
  --text-secondary: #D1D5DB;
  --text-tertiary: #9CA3AF;
  --text-inverse: #0F172A;
  
  /* Background Colors - Dark Mode */
  --bg-primary: #0F172A;
  --bg-secondary: #1E293B;
  --bg-tertiary: #1F2937;
  
  /* Border & Shadow - Dark Mode */
  --border-color: #374151;
  --border-light: #1F2937;
  --border-dark: #4B5563;
  
  /* Gradients - Dark Mode */
  --gradient-blue-to-orange: linear-gradient(135deg, #1E3A8A 0%, #3B82F6 50%, #FF8C42 100%);
  --gradient-smooth-blue-orange: linear-gradient(90deg, #3B82F6 0%, #60A5FA 25%, #FFCF9B 75%, #FF8C42 100%);
  --gradient-button: linear-gradient(135deg, #3B82F6 0%, #60A5FA 100%);
  --gradient-accent: linear-gradient(90deg, #FF8C42 0%, #FFCF9B 100%);
  --gradient-card: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(255, 140, 66, 0.1) 100%);
  --gradient-bg: linear-gradient(180deg, #0F172A 0%, #1E293B 100%);
}
```

---

## TYPOGRAPHY

### Font Families
```css
--font-display: 'Space Grotesk', 'Sora', 'DM Sans', sans-serif;
--font-body: 'Inter', 'Plus Jakarta Sans', 'Aeonik', sans-serif;
--font-mono: 'Courier New', 'Monaco', monospace;
```

### Font Sizes
```css
--font-size-3xl: 48px;    /* H1 - Hero titles */
--font-size-2xl: 36px;    /* H2 - Major sections */
--font-size-xl: 28px;     /* H3 - Subsections */
--font-size-lg: 20px;     /* H4 - Cards, important */
--font-size-md: 16px;     /* Body text - Standard */
--font-size-sm: 14px;     /* Secondary text, UI labels */
--font-size-xs: 12px;     /* Small text, captions */
```

### Font Weights
```css
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--font-weight-extrabold: 800;
```

### Line Heights
```css
--line-height-tight: 1.2;
--line-height-normal: 1.5;
--line-height-relaxed: 1.75;
--line-height-loose: 2;
```

---

## SPACING SYSTEM

### Base Unit: 4px / 8px

```css
--spacing-xs: 4px;
--spacing-sm: 8px;
--spacing-md: 16px;
--spacing-lg: 24px;
--spacing-xl: 32px;
--spacing-2xl: 48px;
--spacing-3xl: 64px;
--spacing-4xl: 80px;

/* Container Widths */
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1400px;
```

---

## MOTION & ANIMATIONS

### Timing

```css
/* Durations */
--duration-fast: 100ms - 150ms;
--duration-normal: 200ms - 300ms;
--duration-slow: 400ms - 500ms;
--duration-slower: 600ms - 800ms;

/* Easing Functions */
--ease-linear: linear;
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);

/* Transitions */
--transition-fast: all 100ms ease-out;
--transition: all 300ms ease-out;
--transition-slow: all 500ms ease-out;
```

### Keyframe Animations

```css
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes slideInDown {
  from { opacity: 0; transform: translateY(-20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes scaleIn {
  from { opacity: 0; transform: scale(0.95); }
  to { opacity: 1; transform: scale(1); }
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

@keyframes shimmer {
  0% { background-position: -1000px 0; }
  100% { background-position: 1000px 0; }
}

@keyframes bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}
```

---

## SHADOW SYSTEM

### Light Mode Shadows
```css
--shadow-xs: 0 1px 2px 0 rgba(15, 76, 117, 0.05);
--shadow-sm: 0 1px 3px 0 rgba(15, 76, 117, 0.1);
--shadow-md: 0 4px 6px -1px rgba(15, 76, 117, 0.1);
--shadow-lg: 0 10px 15px -3px rgba(15, 76, 117, 0.1);
--shadow-xl: 0 20px 25px -5px rgba(15, 76, 117, 0.1);
--shadow-2xl: 0 25px 50px -12px rgba(15, 76, 117, 0.15);
```

### Dark Mode Shadows
```css
html[data-theme="dark"] {
  --shadow-xs: 0 1px 2px 0 rgba(0, 0, 0, 0.3);
  --shadow-sm: 0 1px 3px 0 rgba(0, 0, 0, 0.4);
  --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.5);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.6);
  --shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.7);
  --shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.8);
}
```

---

## BORDER RADIUS

```css
--radius-none: 0;
--radius-sm: 4px;
--radius-md: 6px;
--radius-lg: 8px;
--radius-xl: 12px;
--radius-2xl: 16px;
--radius-full: 9999px;
```

---

## DARK/LIGHT MODE TOGGLE

### HTML Structure
```html
<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI Platform - Design System</title>
</head>
<body>
  <header>
    <button id="theme-toggle" class="theme-toggle" aria-label="Toggle dark mode">
      <span class="sun-icon">☀️</span>
      <span class="moon-icon">🌙</span>
    </button>
  </header>
</body>
</html>
```

### CSS for Toggle Button

```css
.theme-toggle {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border: 1px solid var(--border-color);
  border-radius: var(--radius-md);
  background: var(--bg-secondary);
  color: var(--text-primary);
  cursor: pointer;
  transition: all 200ms ease-out;
  padding: 0;
}

.theme-toggle:hover {
  background: var(--bg-tertiary);
  transform: scale(1.05);
}

.theme-toggle:active {
  transform: scale(0.95);
}

.sun-icon {
  display: block;
  width: 20px;
  height: 20px;
  font-size: 20px;
}

.moon-icon {
  display: none;
  width: 20px;
  height: 20px;
  font-size: 20px;
}

html[data-theme="dark"] .sun-icon {
  display: none;
}

html[data-theme="dark"] .moon-icon {
  display: block;
}

.sun-icon,
.moon-icon {
  transition: transform 300ms ease-out;
}

.theme-toggle:active .sun-icon,
.theme-toggle:active .moon-icon {
  transform: rotate(180deg);
}

/* Smooth theme transition */
html.theme-transitioning,
html.theme-transitioning * {
  transition: background-color 300ms ease-out, 
              color 300ms ease-out, 
              border-color 300ms ease-out !important;
}
```

---

## COMPONENT STYLES

### Button - Primary with Gradient

```css
.button-primary {
  background: var(--gradient-button);
  color: white;
  padding: 10px 16px;
  border-radius: var(--radius-md);
  border: none;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-sm);
  font-family: var(--font-body);
  cursor: pointer;
  transition: var(--transition-fast);
}

.button-primary:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}

.button-primary:active {
  transform: translateY(0);
  box-shadow: var(--shadow-md);
}

.button-primary:disabled {
  opacity: 0.5;
  cursor: not-allowed;
  transform: none;
}
```

### Button - Secondary with Accent Gradient

```css
.button-secondary {
  background: var(--gradient-accent);
  color: white;
  padding: 10px 16px;
  border-radius: var(--radius-md);
  border: none;
  font-weight: var(--font-weight-semibold);
  font-size: var(--font-size-sm);
  cursor: pointer;
  transition: var(--transition-fast);
}

.button-secondary:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}
```

### Button - Outline

```css
.button-outline {
  background: transparent;
  color: var(--primary-blue);
  border: 2px solid var(--primary-blue);
  padding: 8px 14px;
  border-radius: var(--radius-md);
  font-weight: var(--font-weight-semibold);
  cursor: pointer;
  transition: var(--transition-fast);
}

.button-outline:hover {
  background: var(--primary-blue);
  color: white;
  transform: translateY(-2px);
}
```

### Card with Gradient Border

```css
.card {
  background: var(--bg-secondary);
  border-radius: var(--radius-lg);
  padding: var(--spacing-lg);
  box-shadow: var(--shadow-md);
  border: 1px solid var(--border-color);
  transition: var(--transition);
  position: relative;
  overflow: hidden;
}

.card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 3px;
  background: var(--gradient-blue-to-orange);
  opacity: 0;
  transition: opacity 300ms ease-out;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow-lg);
}

.card:hover::before {
  opacity: 1;
}
```

### Input Field

```css
.input {
  width: 100%;
  padding: var(--spacing-md);
  border: 1px solid var(--border-color);
  border-radius: var(--radius-md);
  background: var(--bg-primary);
  color: var(--text-primary);
  font-family: var(--font-body);
  font-size: var(--font-size-sm);
  transition: var(--transition-fast);
}

.input:focus {
  outline: none;
  border-color: var(--primary-blue);
  box-shadow: 0 0 0 3px rgba(31, 58, 147, 0.1);
}

.input::placeholder {
  color: var(--text-tertiary);
}

html[data-theme="dark"] .input:focus {
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.2);
}

.input.error {
  border-color: var(--error);
}

.input.success {
  border-color: var(--success);
}
```

### Message/Chat Bubble

```css
.message {
  display: flex;
  flex-direction: column;
  gap: 4px;
  animation: slideInUp 300ms ease;
}

.message.user {
  align-items: flex-end;
}

.message.ai {
  align-items: flex-start;
}

.message__bubble {
  max-width: 70%;
  padding: 12px 16px;
  border-radius: var(--radius-lg);
  font-size: var(--font-size-sm);
  line-height: var(--line-height-normal);
  word-wrap: break-word;
}

.message.user .message__bubble {
  background: var(--gradient-button);
  color: white;
}

.message.ai .message__bubble {
  background: var(--bg-tertiary);
  color: var(--text-primary);
  border: 1px solid var(--border-color);
}

.message__time {
  font-size: var(--font-size-xs);
  color: var(--text-tertiary);
}
```

### Loading Spinner

```css
.spinner {
  width: 20px;
  height: 20px;
  border: 2px solid var(--border-color);
  border-top-color: var(--primary-blue);
  border-radius: 50%;
  animation: spin 600ms linear infinite;
}

@media (prefers-reduced-motion: reduce) {
  .spinner {
    animation: none;
    opacity: 0.5;
  }
}
```

---

## RESPONSIVE BREAKPOINTS

```css
/* Mobile First Approach */

/* Mobile: 320px - 640px (default) */
@media (min-width: 320px) {
  /* Default mobile styles */
}

/* Small: 640px - 768px */
@media (min-width: 640px) {
  /* Adjustments for small tablets */
}

/* Medium: 768px - 1024px */
@media (min-width: 768px) {
  /* Adjustments for tablets */
}

/* Large: 1024px - 1280px */
@media (min-width: 1024px) {
  /* Desktop layout */
}

/* Extra Large: 1280px+ */
@media (min-width: 1280px) {
  /* Large desktop adjustments */
}
```

### Accessibility - Reduced Motion

```css
@media (prefers-color-scheme: dark) {
  /* Dark mode styles */
}

@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## CSS VARIABLES SUMMARY

```css
/* All Variables in One Place */
:root {
  /* ===== COLORS ===== */
  /* Blues */
  --primary-blue-dark: #0F4C75;
  --primary-blue: #1F3A93;
  --primary-blue-light: #3B82F6;
  --primary-blue-lighter: #60A5FA;
  
  /* Oranges */
  --accent-orange: #FF6B35;
  --accent-orange-light: #FF8C42;
  --accent-orange-pale: #FFCF9B;
  
  /* Neutrals */
  --neutral-white: #FFFFFF;
  --neutral-50: #F9FAFB;
  --neutral-100: #F3F4F6;
  --neutral-200: #E5E7EB;
  --neutral-700: #1F2937;
  
  /* Semantic */
  --success: #10B981;
  --warning: #F59E0B;
  --error: #EF4444;
  
  /* Text */
  --text-primary: #1F2937;
  --text-secondary: #6B7280;
  --text-tertiary: #9CA3AF;
  
  /* Background */
  --bg-primary: #FFFFFF;
  --bg-secondary: #F9FAFB;
  --bg-tertiary: #F3F4F6;
  
  /* Borders */
  --border-color: #E5E7EB;
  
  /* ===== GRADIENTS ===== */
  --gradient-blue-to-orange: linear-gradient(135deg, #0F4C75 0%, #3B82F6 50%, #FF6B35 100%);
  --gradient-button: linear-gradient(135deg, #1F3A93 0%, #3B82F6 100%);
  --gradient-accent: linear-gradient(90deg, #FF6B35 0%, #FF8C42 100%);
  
  /* ===== TYPOGRAPHY ===== */
  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'Inter', sans-serif;
  --font-size-md: 16px;
  --font-weight-semibold: 600;
  --line-height-normal: 1.5;
  
  /* ===== SPACING ===== */
  --spacing-xs: 4px;
  --spacing-sm: 8px;
  --spacing-md: 16px;
  --spacing-lg: 24px;
  --spacing-xl: 32px;
  --spacing-2xl: 48px;
  
  /* ===== MOTION ===== */
  --transition: all 300ms ease-out;
  --transition-fast: all 150ms ease-out;
  
  /* ===== SHADOWS ===== */
  --shadow-sm: 0 1px 3px 0 rgba(15, 76, 117, 0.1);
  --shadow-md: 0 4px 6px -1px rgba(15, 76, 117, 0.1);
  --shadow-lg: 0 10px 15px -3px rgba(15, 76, 117, 0.1);
  
  /* ===== RADIUS ===== */
  --radius-md: 6px;
  --radius-lg: 8px;
}
```

---

## HTML TEMPLATE

```html
<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI Platform</title>
  <style>
    /* ALL CSS VARIABLES AND STYLES ABOVE */
  </style>
</head>
<body>
  <header>
    <div class="container header__container">
      <a href="/" class="logo">AI Platform</a>
      
      <nav class="header__nav">
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#pricing">Pricing</a>
        <a href="#about">About</a>
      </nav>
      
      <button id="theme-toggle" class="theme-toggle" aria-label="Toggle dark mode">
        <span class="sun-icon">☀️</span>
        <span class="moon-icon">🌙</span>
      </button>
    </div>
  </header>

  <main class="container">
    <!-- Hero Section -->
    <section class="hero">
      <h1>Welcome to AI Platform</h1>
      <p>Advanced AI models with Sarvam-inspired design</p>
      <button class="button-primary">Get Started</button>
    </section>

    <!-- Features Section -->
    <section class="features">
      <h2>Features</h2>
      <div class="grid">
        <div class="card">
          <h3>Advanced Models</h3>
          <p>State-of-the-art language models</p>
        </div>
        <div class="card">
          <h3>Secure Design</h3>
          <p>Enterprise-grade security</p>
        </div>
        <div class="card">
          <h3>Easy Deployment</h3>
          <p>Deploy anywhere with ease</p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 AI Platform. All rights reserved.</p>
  </footer>

  <script>
    // JAVASCRIPT CODE BELOW
  </script>
</body>
</html>
```

---

## JAVASCRIPT IMPLEMENTATION

```javascript
// Dark/Light Mode Toggle

// Check for saved theme preference or system preference
const currentTheme = localStorage.getItem('theme') || 
  (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light');

// Set initial theme
document.documentElement.setAttribute('data-theme', currentTheme);

// Get toggle button
const themeToggle = document.getElementById('theme-toggle');

// Toggle theme on button click
themeToggle.addEventListener('click', () => {
  const html = document.documentElement;
  const currentTheme = html.getAttribute('data-theme');
  const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
  
  // Add transition class
  html.classList.add('theme-transitioning');
  
  // Change theme
  html.setAttribute('data-theme', newTheme);
  localStorage.setItem('theme', newTheme);
  
  // Remove transition class after animation
  setTimeout(() => {
    html.classList.remove('theme-transitioning');
  }, 300);
});

// Listen for system theme changes
window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', (e) => {
  const newTheme = e.matches ? 'dark' : 'light';
  document.documentElement.setAttribute('data-theme', newTheme);
  localStorage.setItem('theme', newTheme);
});

// Optional: Smooth scroll behavior
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function (e) {
    e.preventDefault();
    const target = document.querySelector(this.getAttribute('href'));
    if (target) {
      target.scrollIntoView({ behavior: 'smooth' });
    }
  });
});
```

---

## QUICK START GUIDE

### Step 1: Copy CSS Variables
Copy the entire `:root` section and `html[data-theme="dark"]` section to your main CSS file.

### Step 2: Add Theme Toggle Button
```html
<button id="theme-toggle" class="theme-toggle">
  <span class="sun-icon">☀️</span>
  <span class="moon-icon">🌙</span>
</button>
```

### Step 3: Add Toggle CSS
Copy the `.theme-toggle` styles above.

### Step 4: Add JavaScript
Copy the JavaScript implementation above to enable theme switching.

### Step 5: Use Variables in Your Styles
```css
.my-button {
  background: var(--gradient-button);
  color: white;
  transition: var(--transition);
}

.my-button:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}
```

---

## COLOR QUICK REFERENCE

| Element | Light Mode | Dark Mode |
|---------|-----------|----------|
| **Primary Button** | #1F3A93 | #3B82F6 |
| **Accent Button** | #FF6B35 | #FF8C42 |
| **Background** | #FFFFFF | #0F172A |
| **Text Primary** | #1F2937 | #F3F4F6 |
| **Text Secondary** | #6B7280 | #D1D5DB |
| **Border** | #E5E7EB | #374151 |

---

## MOTION TIMING QUICK REFERENCE

| Element | Duration | Easing |
|---------|----------|--------|
| **Hover State** | 150ms | ease-out |
| **Page Transition** | 300ms | ease-out |
| **Modal Open** | 300ms | ease-out |
| **Spinner** | 600ms | linear |
| **Shimmer** | 2s | linear |

---

## ACCESSIBILITY CHECKLIST

- ✅ Dark mode support via `prefers-color-scheme`
- ✅ Respects `prefers-reduced-motion` preference
- ✅ WCAG color contrast ratios (4.5:1)
- ✅ Semantic HTML structure
- ✅ ARIA labels for interactive elements
- ✅ Keyboard navigation support
- ✅ Focus visible indicators
- ✅ Sufficient spacing for touch targets

---

## USAGE TIPS

1. **Always use CSS variables** for consistency
2. **Test both light and dark modes** during development
3. **Use gradients for visual interest** in hero sections and CTAs
4. **Animate thoughtfully** - use motion to guide, not distract
5. **Test with system dark mode preferences**
6. **Respect user motion preferences** - don't force animations
7. **Test contrast ratios** especially in dark mode
8. **Use semantic HTML** for accessibility

---

## FONTS TO INSTALL

Add to your HTML `<head>`:

```html
<!-- Display Font -->
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">

<!-- Body Font -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

Or use CDN imports in your CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
```

---

## COMPLETE EXAMPLE

See working example with all components:

```html
<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AI Platform - Complete Example</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      /* All variables from above */
      --primary-blue: #1F3A93;
      --accent-orange: #FF6B35;
      --text-primary: #1F2937;
      --bg-primary: #FFFFFF;
      --gradient-button: linear-gradient(135deg, #1F3A93 0%, #3B82F6 100%);
      --transition: all 300ms ease-out;
      --spacing-lg: 24px;
      --font-display: 'Space Grotesk', sans-serif;
      --font-body: 'Inter', sans-serif;
    }

    html[data-theme="dark"] {
      --primary-blue: #3B82F6;
      --accent-orange: #FF8C42;
      --text-primary: #F3F4F6;
      --bg-primary: #0F172A;
      --gradient-button: linear-gradient(135deg, #3B82F6 0%, #60A5FA 100%);
    }

    body {
      font-family: var(--font-body);
      color: var(--text-primary);
      background: var(--bg-primary);
      transition: var(--transition);
    }

    .button-primary {
      background: var(--gradient-button);
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      transition: var(--transition);
      font-weight: 600;
    }

    .button-primary:hover {
      transform: translateY(-2px);
    }

    .theme-toggle {
      background: none;
      border: none;
      font-size: 24px;
      cursor: pointer;
    }

    .moon-icon {
      display: none;
    }

    html[data-theme="dark"] .sun-icon {
      display: none;
    }

    html[data-theme="dark"] .moon-icon {
      display: block;
    }
  </style>
</head>
<body>
  <header style="padding: 20px; display: flex; justify-content: space-between; align-items: center;">
    <h1 style="font-family: var(--font-display);">AI Platform</h1>
    <button id="theme-toggle" class="theme-toggle">
      <span class="sun-icon">☀️</span>
      <span class="moon-icon">🌙</span>
    </button>
  </header>

  <main style="max-width: 1200px; margin: 0 auto; padding: var(--spacing-lg);">
    <h2 style="margin-bottom: var(--spacing-lg); color: var(--primary-blue);">Welcome</h2>
    <p style="margin-bottom: var(--spacing-lg);">This is a complete design system with dark/light mode support.</p>
    <button class="button-primary">Get Started</button>
  </main>

  <script>
    const themeToggle = document.getElementById('theme-toggle');
    const currentTheme = localStorage.getItem('theme') || 'light';
    document.documentElement.setAttribute('data-theme', currentTheme);

    themeToggle.addEventListener('click', () => {
      const html = document.documentElement;
      const newTheme = html.getAttribute('data-theme') === 'dark' ? 'light' : 'dark';
      html.setAttribute('data-theme', newTheme);
      localStorage.setItem('theme', newTheme);
    });
  </script>
</body>
</html>
```

---

## SUPPORT & DOCUMENTATION

**Color Palette**: Based on Sarvam.ai design system with blue-to-orange gradient spectrum

**Typography**: Space Grotesk (display) + Inter (body)

**Motion**: Smooth 300ms transitions with ease-out easing

**Dark Mode**: Complete color override with CSS variables

**Responsive**: Mobile-first, breakpoints at 640px, 768px, 1024px, 1280px

---

**This is your complete, all-in-one design system reference. Copy, paste, and customize!** 🎉

