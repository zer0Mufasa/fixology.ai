# Fixology Design System
## Version 2.0 - Lavender Tech Theme

---

## 🎨 Color Palette

### Primary - Lavender Gradient
```css
--lavender-100: #E8E0FF;  /* Lightest */
--lavender-200: #D4C4FF;
--lavender-300: #B48FFF;  /* Primary accent */
--lavender-400: #8E75FF;  /* Main brand */
--lavender-500: #6B59FF;  /* Dark accent */
--lavender-600: #5344CC;  /* Darkest */

/* Gradient */
--gradient-lavender: linear-gradient(135deg, #B48FFF 0%, #8E75FF 50%, #6B59FF 100%);
```

### Accent - Neon Cyan
```css
--cyan-glow: #6DF7FF;     /* Primary cyan */
--cyan-dim: #4ED8E0;      /* Dimmed cyan */

/* Gradient */
--gradient-cyan: linear-gradient(135deg, #6DF7FF 0%, #4ED8E0 100%);
```

### Backgrounds (Dark Mode)
```css
--bg-primary: #07070A;    /* Main background */
--bg-secondary: #0D0D12;  /* Section backgrounds */
--bg-tertiary: #131318;   /* Elevated surfaces */
--bg-card: #18181F;       /* Card backgrounds */
--bg-card-hover: #1E1E26; /* Card hover state */
```

### Text
```css
--text-primary: #FFFFFF;   /* Headings, important text */
--text-secondary: #A0A0B0; /* Body text */
--text-tertiary: #6B6B7B;  /* Muted text, labels */
```

### Borders
```css
--border-subtle: rgba(255, 255, 255, 0.06);  /* Subtle dividers */
--border-medium: rgba(255, 255, 255, 0.1);   /* Card borders */
```

### Status Colors
```css
--success: #28C840;  /* Green - complete, success */
--warning: #FEBC2E;  /* Yellow - in progress, warning */
--danger: #FF6B6B;   /* Red - error, danger */
--info: #6DF7FF;     /* Cyan - info, new */
```

---

## 📝 Typography

### Font Family
```css
--font-main: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

### Font Sizes
```css
/* Display */
.text-display: 4.5rem;    /* 72px - Hero headlines */
.text-h1: 3rem;           /* 48px - Page titles */
.text-h2: 2.25rem;        /* 36px - Section titles */
.text-h3: 1.5rem;         /* 24px - Card titles */
.text-h4: 1.125rem;       /* 18px - Subsection titles */

/* Body */
.text-lg: 1.125rem;       /* 18px - Lead paragraphs */
.text-base: 0.9375rem;    /* 15px - Body text */
.text-sm: 0.875rem;       /* 14px - Secondary text */
.text-xs: 0.8125rem;      /* 13px - Labels */
.text-xxs: 0.75rem;       /* 12px - Badges, tiny text */
```

### Font Weights
```css
--font-light: 300;
--font-normal: 400;
--font-medium: 500;
--font-semibold: 600;
--font-bold: 700;
--font-extrabold: 800;
```

### Letter Spacing
```css
/* Headings: Tight */
h1, h2: letter-spacing: -1.5px to -1px;
h3, h4: letter-spacing: -0.5px to -0.3px;

/* Labels: Wide */
.label: letter-spacing: 1px to 1.5px;
```

---

## 📐 Spacing

### Base Scale (rem)
```css
--space-xs: 0.25rem;   /* 4px */
--space-sm: 0.5rem;    /* 8px */
--space-md: 1rem;      /* 16px */
--space-lg: 1.5rem;    /* 24px */
--space-xl: 2rem;      /* 32px */
--space-2xl: 3rem;     /* 48px */
--space-3xl: 4rem;     /* 64px */
--space-4xl: 6rem;     /* 96px */
--space-5xl: 8rem;     /* 128px */
```

### Section Padding
```css
section { padding: 6rem 2rem; }  /* Desktop */
section { padding: 4rem 1.5rem; } /* Mobile */
```

### Container Max Widths
```css
--container-sm: 600px;
--container-md: 800px;
--container-lg: 1000px;
--container-xl: 1200px;
--container-full: 1400px;
```

---

## 🔲 Components

### Buttons
```css
/* Base */
.btn {
  padding: 0.625rem 1.25rem;
  border-radius: 8px;
  font-size: 0.875rem;
  font-weight: 500;
  transition: all 0.2s ease;
}

/* Primary - Gradient with glow */
.btn-primary {
  background: var(--gradient-lavender);
  color: white;
  box-shadow: 0 0 20px rgba(142, 117, 255, 0.3);
}
.btn-primary:hover {
  transform: translateY(-1px);
  box-shadow: 0 0 30px rgba(142, 117, 255, 0.4);
}

/* Secondary - Dark with border */
.btn-secondary {
  background: var(--bg-card);
  color: white;
  border: 1px solid var(--border-medium);
}

/* Ghost - Transparent */
.btn-ghost {
  background: transparent;
  color: var(--text-secondary);
}

/* Large */
.btn-lg {
  padding: 0.875rem 1.75rem;
  font-size: 0.9375rem;
}
```

### Cards
```css
.card {
  background: var(--bg-card);
  border: 1px solid var(--border-subtle);
  border-radius: 16px;
  padding: 1.5rem;
  transition: all 0.3s ease;
}
.card:hover {
  border-color: var(--lavender-500);
  transform: translateY(-4px);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
}
```

### Badges
```css
.badge {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.375rem 0.875rem;
  background: rgba(142, 117, 255, 0.1);
  border: 1px solid rgba(142, 117, 255, 0.2);
  border-radius: 100px;
  font-size: 0.8125rem;
  color: var(--lavender-300);
}

/* With dot indicator */
.badge-dot {
  width: 6px;
  height: 6px;
  background: var(--cyan-glow);
  border-radius: 50%;
  box-shadow: 0 0 10px var(--cyan-glow);
}
```

### Form Inputs
```css
.input {
  width: 100%;
  padding: 0.875rem 1rem;
  background: var(--bg-secondary);
  border: 1px solid var(--border-subtle);
  border-radius: 10px;
  color: var(--text-primary);
  font-size: 0.9375rem;
  transition: border-color 0.2s;
}
.input:focus {
  outline: none;
  border-color: var(--lavender-400);
}
.input::placeholder {
  color: var(--text-tertiary);
}
```

### Status Tags
```css
.status {
  padding: 0.25rem 0.625rem;
  border-radius: 100px;
  font-size: 0.75rem;
  font-weight: 500;
}
.status-new { background: rgba(142,117,255,0.15); color: var(--lavender-300); }
.status-progress { background: rgba(254,188,46,0.15); color: #FEBC2E; }
.status-complete { background: rgba(40,200,64,0.15); color: #28C840; }
.status-waiting { background: rgba(109,247,255,0.15); color: var(--cyan-glow); }
```

---

## ✨ Effects

### Shadows
```css
/* Subtle */
.shadow-sm: 0 4px 12px rgba(0, 0, 0, 0.1);

/* Medium */
.shadow-md: 0 20px 40px rgba(0, 0, 0, 0.2);

/* Large */
.shadow-lg: 0 40px 80px rgba(0, 0, 0, 0.4);

/* Glow (for primary elements) */
.shadow-glow: 0 0 30px rgba(142, 117, 255, 0.3);
```

### Background Effects
```css
/* Hero gradient glow */
.hero-glow {
  background: radial-gradient(
    ellipse at 50% 0%, 
    rgba(142, 117, 255, 0.15) 0%, 
    transparent 50%
  );
}

/* Grid pattern */
.grid-pattern {
  background-image: 
    linear-gradient(rgba(142, 117, 255, 0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(142, 117, 255, 0.03) 1px, transparent 1px);
  background-size: 80px 80px;
}

/* Glassmorphism (navigation) */
.glass {
  background: rgba(7, 7, 10, 0.8);
  backdrop-filter: blur(20px);
}
```

### Animations
```css
/* Fade up */
@keyframes fade-up {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

/* Pulse glow */
@keyframes pulse-glow {
  0%, 100% { opacity: 0.5; transform: scale(1); }
  50% { opacity: 0.8; transform: scale(1.1); }
}

/* Blink (status indicators) */
@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.4; }
}
```

---

## 📱 Responsive Breakpoints

```css
/* Mobile first approach */
@media (min-width: 640px) { /* sm */ }
@media (min-width: 768px) { /* md */ }
@media (min-width: 1024px) { /* lg */ }
@media (min-width: 1280px) { /* xl */ }
@media (min-width: 1536px) { /* 2xl */ }
```

---

## 🏗️ Layout Patterns

### Section Header
```html
<div class="section-header">
  <div class="section-label">LABEL TEXT</div>
  <h2 class="section-title">Section Title Here</h2>
  <p class="section-subtitle">Supporting description text.</p>
</div>
```

### Grid Layouts
```css
/* 4-column features */
.features-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1rem;
}

/* 3-column pricing */
.pricing-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
}

/* 2-column content */
.two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
}
```

---

## 🎯 Icon System

Using emoji icons for simplicity. Key icons:

| Use Case | Icon |
|----------|------|
| Diagnostic | 🧠 |
| POS | 🧾 |
| Inventory | 📦 |
| Training | 📚 |
| Analytics | 📊 |
| Settings | ⚙️ |
| Customer | 👤 |
| Shop | 🏪 |
| Success | ✅ |
| Warning | ⚠️ |
| Money | 💰 |
| Device | 📱 |

---

## 📄 Page Structure

```
├── Navigation (fixed, glass effect)
├── Hero Section
│   ├── Badge
│   ├── Title (with gradient text)
│   ├── Subtitle
│   └── CTA buttons
├── Content Sections
│   ├── Section Header
│   └── Content (grid/cards/text)
├── CTA Section
└── Footer
```

---

## 🚀 Implementation Notes

1. **Font Loading**: Use `font-display: swap` for Inter
2. **Images**: Use WebP with fallbacks, lazy load below fold
3. **Animations**: Respect `prefers-reduced-motion`
4. **Dark Mode**: This IS the default (no light mode needed)
5. **Accessibility**: Maintain 4.5:1 contrast ratio minimum
