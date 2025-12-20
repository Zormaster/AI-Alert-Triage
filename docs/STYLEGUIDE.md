# Gnostyx - Design Styleguide

This styleguide documents the design tokens, color palette, and UI components used in the Gnostyx landing page.

## Design Philosophy
- **Theme:** Dark, Technical, "Cybersecurity SaaS"
- **Base Framework:** Tailwind CSS
- **Primary Font:** Inter
- **Mood:** Professional, trustworthy, high-tech, clean

---

## Color Palette

### Brand Colors (Primary)
Used for primary actions, highlights, and branding elements.
- **Brand 50:** `#eff6ff` (Background accents)
- **Brand 100:** `#dbeafe`
- **Brand 200:** `#bfdbfe`
- **Brand 300:** `#93c5fd`
- **Brand 400:** `#60a5fa` (Text highlights, icon accents)
- **Brand 500:** `#3b82f6` (Primary buttons, active states)
- **Brand 600:** `#2563eb` (Hover states)
- **Brand 700:** `#1d4ed8`
- **Brand 800:** `#1e40af`
- **Brand 900:** `#1e3a8a`
- **Brand 950:** `#172554`

### Neutral Colors (Slate)
Used for backgrounds, text, and borders to maintain a cool, dark technical feel.
- **Background:** `bg-slate-950` (Main Page Background)
- **Surface:** `bg-slate-900` (Cards, Sections)
- **Border:** `border-slate-800`
- **Text Primary:** `text-white` / `text-slate-50`
- **Text Secondary:** `text-slate-300` / `text-slate-400`
- **Text Muted:** `text-slate-500`

### Semantic Colors
- **Success:** Green-500 (Live status, indicators)
- **Warning:** Yellow-500 (Analysis indicators)
- **Danger:** Red-500 (Critical alerts, Priority: High)
- **Info:** Blue-500 (General status)

---

## Typography

**Font Family:** Inter (`sans-serif`)

### Hierarchy
- **H1 (Hero):** `text-5xl md:text-7xl font-bold tracking-tight text-white`
- **H2 (Section):** `text-3xl font-bold text-white`
- **H3 (Card Title):** `text-xl font-bold text-white` / `text-2xl font-bold`
- **Body Large:** `text-xl text-slate-400`
- **Body Regular:** `text-base text-slate-300`
- **Small/Label:** `text-sm font-medium text-slate-400`

---

## UI Components

### Buttons
**Primary Action (Get Early Access):**
```html
<button class="px-8 py-4 rounded-full bg-brand-600 text-white font-semibold text-lg hover:bg-brand-500 transition-all shadow-lg shadow-brand-900/40 border border-transparent">
```

**Secondary Action (See How It Works):**
```html
<button class="px-8 py-4 rounded-full bg-slate-900 text-slate-300 border border-slate-700 font-semibold text-lg hover:bg-slate-800 hover:text-white transition-all">
```

**Nav Link:**
```html
<a class="px-3 py-2 rounded-md text-sm font-medium text-slate-400 hover:text-brand-400 transition-colors">
```

### Cards
**Feature Card:**
- **Background:** `bg-slate-900`
- **Border:** `border border-slate-800`
- **Hover:** `hover:border-brand-500/30` (or specific color variant)
- **Shadow:** `shadow-sm hover:shadow-lg`
- **Rounding:** `rounded-2xl`

### Badges / Pills
**Status Badge:**
```html
<span class="text-xs font-semibold uppercase tracking-wider text-green-400 bg-green-500/10 border border-green-500/20 px-2 py-1 rounded-full">
    Live
</span>
```

**Early Access Label:**
```html
<div class="inline-flex items-center px-3 py-1 rounded-full bg-brand-900/30 border border-brand-700/50 text-brand-300 text-sm font-medium">
```

### Form Elements
**Input Field:**
```html
<input class="rounded-md border-0 bg-white/5 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-brand-500 sm:text-sm sm:leading-6">
```

---

## Effects

### Gradients & Glows
- **Text Gradient:** `bg-clip-text text-transparent bg-gradient-to-r from-brand-400 to-purple-400`
- **Background Blobs:** `mix-blend-screen filter blur-[128px]`
- **Section Glow:** `bg-[radial-gradient(45rem_50rem_at_top,theme(colors.brand.900),theme(colors.slate.950))]`

### Scrollbar
Custom dark scrollbar overrides default browser styling.
- **Track:** `#020617`
- **Thumb:** `#1e293b` (Hover: `#334155`)
