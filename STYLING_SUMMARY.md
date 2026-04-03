# Arc Raiders Website - Premium Styling Enhancements

## Summary of Changes

### 1. CSS Foundation (Complete Rewrite)
**File:** `css/style.css` (41KB)

#### Design System
- **CSS Custom Properties**: Full design token system with colors, typography, spacing, shadows
- **Dark/Light Theme Variables**: Complete color palette for both themes
- **Responsive Typography**: Fluid font sizing using `clamp()`
- **Consistent Spacing**: 8-point spacing scale

#### Key Features
- **Smooth Animations**: CSS transitions with cubic-bezier easing
- **Gradient Accents**: Orange-to-gold gradient for premium feel
- **Glow Effects**: Subtle accent glows for interactive elements
- **Card Hover States**: Lift, glow, and border accent animations

### 2. Dark/Light Mode Toggle
**Auto-Generated Button**

- Floating theme toggle button (bottom-right corner)
- Saves preference to localStorage
- Respects system preference on first visit
- Smooth icon animation between sun/moon
- Accessible with ARIA labels

### 3. Animations & Micro-interactions

#### Page Load Animations
- Hero content fade-in-up
- Stats counter animation
- Staggered card entrance animations

#### Hover Effects
- Card lift with subtle rotation
- Button gradient shine effect
- Navigation underline slide-in
- Link color transitions

#### Continuous Animations
- Hero grid parallax movement
- Pulse glow on logo icon
- Badge glow breathing effect
- Icon floating animation

### 4. Mobile Responsiveness

#### Breakpoints
- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

#### Mobile-First Features
- Responsive navigation (hamburger menu)
- Stacked card layouts
- Touch-friendly button sizes
- Flexible grid systems
- Hide/show navbar on scroll (mobile)

### 5. Typography Improvements

#### Font Stack
- **Display**: Rajdhani (headings, numbers)
- **Body**: Inter (paragraphs, UI text)

#### Hierarchy
- Fluid heading sizes with `clamp()`
- Proper line-height for readability
- Letter-spacing on labels and badges

### 6. Accessibility Features

#### ARIA Labels
- Skip to content link (keyboard navigation)
- Navigation toggle states
- Button labels

#### Focus States
- Visible focus rings on all interactive elements
- Focus-visible for keyboard-only highlighting

#### Motion Preferences
- `prefers-reduced-motion` media query support
- Respects user animation preferences

#### Color Contrast
- High contrast mode support
- WCAG compliant color combinations

### 7. JavaScript Enhancements
**File:** `js/main.js` (18KB)

#### Modules
1. **ThemeManager**: Dark/light mode with localStorage persistence
2. **AnimationObserver**: Intersection Observer for scroll animations
3. **MobileNav**: Hamburger menu with accessibility
4. **NavbarScroll**: Scroll-based navbar effects
5. **SmoothScroll**: Anchor link smooth scrolling
6. **WeaponFilters**: Category/rarity filtering with debounce
7. **StatsCounter**: Animated number counting
8. **Tabs**: Tab panel functionality
9. **Toast**: Notification system

### 8. All HTML Pages Updated
- `index.html`
- `weapons.html`
- `maps.html`
- `crafting.html`
- `extraction.html`
- `guides.html`
- `404.html`
- `beginner-tips.html`
- `enemies.html`
- `loot.html`
- `news.html`
- `skills.html`

#### Changes per Page
- Skip to content link added
- Navigation accessibility attributes
- Main content IDs for skip links

## Design Reference

### Color Palette (Dark)
- **Background Primary**: #0a0b0f (near-black)
- **Background Secondary**: #111218 (charcoal)
- **Background Card**: #15171e (card backgrounds)
- **Accent**: #ff6b35 (tactical orange)
- **Gold**: #d4a853 (premium gold)
- **Text Primary**: #f5f3ef (off-white)
- **Text Secondary**: #9ca3af (muted gray)

### Color Palette (Light)
- **Background Primary**: #f8f7f5 (warm white)
- **Background Card**: #ffffff (pure white)
- **Text Primary**: #1a1c24 (near-black)
- Same accent colors as dark mode

## Browser Support
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimizations
- CSS custom properties for efficient theming
- Intersection Observer for scroll animations
- Debounced search/filter inputs
- Passive event listeners for scroll
- `will-change` hints for animated properties
