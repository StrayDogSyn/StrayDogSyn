# GitHub Profile Design System Reference

## 🎨 Color Palette

### Brand Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| **Hunter Green** | `#355E3B` | `rgb(53, 94, 59)` | Primary brand, links, accents |
| **Dark Canvas** | `#0d1117` | `rgb(13, 17, 23)` | Dark mode background |
| **Light Canvas** | `#ffffff` | `rgb(255, 255, 255)` | Light mode background |
| **Dark Surface** | `#1e1e1e` | `rgb(30, 30, 30)` | Secondary dark surfaces |
| **Light Surface** | `#f6f8fa` | `rgb(246, 248, 250)` | Secondary light surfaces |

### Semantic Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| **Success Green** | `#28a745` | `rgb(40, 167, 69)` | Success states, availability |
| **Danger Red** | `#dc3545` | `rgb(220, 53, 69)` | Errors, warnings |
| **Info Blue** | `#17a2b8` | `rgb(23, 162, 184)` | Informational messages |
| **Warning Yellow** | `#ffc107` | `rgb(255, 193, 7)` | Caution states |

### Text Colors

| Color Name | Hex Code | RGB | Usage |
|------------|----------|-----|-------|
| **Dark Text** | `#000000` | `rgb(0, 0, 0)` | Primary text (light mode) |
| **Light Text** | `#c9d1d9` | `rgb(201, 209, 217)` | Primary text (dark mode) |
| **Muted Text** | `#6c757d` | `rgb(108, 117, 125)` | Secondary text |
| **White Text** | `#ffffff` | `rgb(255, 255, 255)` | Text on dark backgrounds |

### Technology Colors (Badges)

| Technology | Hex Code | Usage |
|------------|----------|-------|
| **JavaScript** | `#F7DF1E` | JavaScript badges |
| **TypeScript** | `#3178C6` | TypeScript badges |
| **Python** | `#3776AB` | Python badges |
| **React** | `#61DAFB` | React badges |
| **Node.js** | `#339933` | Node.js badges |
| **MongoDB** | `#47A248` | MongoDB badges |
| **GitHub** | `#181717` | GitHub badges |
| **Vercel** | `#000000` | Vercel badges |

### Social Platform Colors

| Platform | Hex Code | Usage |
|----------|----------|-------|
| **LinkedIn** | `#0A66C2` | LinkedIn badges |
| **Gmail** | `#EA4335` | Email badges |
| **Hugging Face** | `#FFD21E` | Hugging Face badges |
| **CodeWars** | `#B1361E` | CodeWars badges |
| **LeetCode** | `#FFA116` | LeetCode badges |
| **HackerRank** | `#00EA64` | HackerRank badges |
| **Kaggle** | `#20BEFF` | Kaggle badges |

---

## 🔤 Typography

### Font Families

```css
/* System Font Stack (Default) */
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", 
             Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji";

/* Monospace (Code) */
font-family: "JetBrains Mono", ui-monospace, SFMono-Regular, "SF Mono", 
             Menlo, Consolas, "Liberation Mono", monospace;
```

### Heading Hierarchy

| Level | Markdown | Size (approx) | Usage |
|-------|----------|---------------|-------|
| **H1** | `#` | 32-48px | Page title, name |
| **H2** | `##` | 24-36px | Major sections |
| **H3** | `###` | 18-24px | Subsections |
| **H4** | `####` | 16-18px | Minor headings |

### Type Scale

```markdown
# H1 - Main Identity (32-48px)
Your Name / Primary Header

## H2 - Section Headers (24-36px)
Professional Experience, Projects, Skills

### H3 - Subsection Headers (18-24px)
Individual Job Titles, Project Names

#### H4 - Detail Headers (16-18px)
Certification Categories, Minor Details

Body Text (14-16px)
Regular paragraph content, descriptions

Small Text (12-14px)
Captions, metadata, footer information
```

### Font Weights

| Weight | Value | Usage |
|--------|-------|-------|
| **Regular** | 400 | Body text |
| **Medium** | 500 | Emphasized text |
| **Semibold** | 600 | Subheadings, important text |
| **Bold** | 700 | Headers, strong emphasis |

---

## 📏 Spacing System

### Vertical Spacing (Line Breaks)

```markdown
<!-- Between major sections -->
---
(3 line breaks = ~48px)

<!-- Between subsections -->
(2 line breaks = ~32px)

<!-- Between paragraphs -->
(1 line break = ~16px)

<!-- Within content blocks -->
<br> (explicit break = ~8px)
```

### Padding & Margins

| Size | Value | Usage |
|------|-------|-------|
| **XS** | 4px | Tight spacing |
| **SM** | 8px | Small gaps |
| **MD** | 16px | Standard spacing |
| **LG** | 24px | Section spacing |
| **XL** | 32px | Major section spacing |
| **2XL** | 48px | Between major blocks |

---

## 🎯 Badge Design System

### Badge Styles

#### For-the-Badge (Primary Style)
```markdown
![Badge](https://img.shields.io/badge/TEXT-355E3B?style=for-the-badge&logo=LOGO&logoColor=white)
```

**Characteristics:**
- Height: 28px
- Font: Bold, all caps
- Padding: 10px horizontal
- Border radius: 4px
- Use for: Status, tech stack, major links

#### Flat-Square (Secondary Style)
```markdown
![Badge](https://img.shields.io/badge/TEXT-355E3B?style=flat-square&logo=LOGO&logoColor=white)
```

**Characteristics:**
- Height: 20px
- Font: Regular, mixed case
- No border radius
- Use for: Stats, metrics, compact info

### Badge Anatomy

```
[LABEL] [MESSAGE]
   ↓        ↓
Logo Text | Value
```

**Components:**
- **Label**: Category or type (optional)
- **Message**: Main content
- **Logo**: Icon/symbol (optional)
- **Color**: Background color (hex without #)
- **Logo Color**: Icon color (usually white/black)

### Common Badge Patterns

#### Status Badge
```markdown
![Status](https://img.shields.io/badge/Status-Active-28a745?style=for-the-badge&labelColor=1e1e1e)
```

#### Technology Badge
```markdown
![Tech](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
```

#### Social Link Badge
```markdown
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](URL)
```

#### Metric Badge
```markdown
![Metric](https://img.shields.io/badge/GPA-3.40%2F4.0-355E3B?style=for-the-badge)
```

---

## 🖼️ Image Guidelines

### Profile/Logo Images

| Type | Dimensions | Format | Max Size |
|------|------------|--------|----------|
| **Header Logo** | 400-600px wide | PNG/SVG | 200KB |
| **Profile Photo** | 400x400px | PNG/JPG | 100KB |
| **Project Screenshot** | 1200x630px | PNG/JPG | 500KB |
| **Icons** | 40-60px | SVG/PNG | 10KB |

### Image Optimization

```markdown
<!-- Responsive Image -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="dark.png">
  <source media="(prefers-color-scheme: light)" srcset="light.png">
  <img alt="Description" src="default.png" width="400" />
</picture>

<!-- Standard Image with Alt Text -->
![Alt Text](url) <!-- Auto-sized -->
<img src="url" alt="Alt Text" width="400" /> <!-- Explicit size -->
```

### Image Best Practices

✅ **Do:**
- Compress images (use tools like TinyPNG)
- Use WebP format when possible
- Include descriptive alt text
- Set explicit width for consistency
- Use SVG for logos/icons
- Host on reliable CDN

❌ **Don't:**
- Use images over 500KB
- Forget alt text
- Use low-resolution images
- Rely on external hotlinks
- Include sensitive information

---

## 🔗 Link Styles

### Primary Links (Badges)
```markdown
[![Text](badge-url)](destination-url)
```

**Use for:**
- Social profiles
- External portfolios
- Live demos
- Source code

### Secondary Links (Inline)
```markdown
[Link Text](url)
```

**Use for:**
- In-text references
- Resource links
- Documentation

### Call-to-Action Links
```markdown
**[📞 Contact Me](mailto:email)**
```

**Use for:**
- Important actions
- Contact requests
- Application links

---

## 📐 Layout Patterns

### Centered Content
```markdown
<div align="center">

Content here...

</div>
```

**Use for:**
- Hero section
- Key stats
- Call-to-action
- Visual emphasis

### Two-Column Layout
```markdown
<table>
<tr>
<td width="50%" valign="top">

Left column...

</td>
<td width="50%" valign="top">

Right column...

</td>
</tr>
</table>
```

**Use for:**
- Experience cards
- Project comparison
- Skills vs certifications

### Three-Column Layout
```markdown
<table>
<tr>
<td align="center" width="33%">

Column 1...

</td>
<td align="center" width="33%">

Column 2...

</td>
<td align="center" width="33%">

Column 3...

</td>
</tr>
</table>
```

**Use for:**
- Coding platform stats
- Technology categories
- Multiple metrics

### Collapsible Section
```markdown
<details>
<summary><b>📁 Section Title</b></summary>
<br>

Hidden content...

</details>
```

**Use for:**
- Long lists
- Optional details
- Certifications
- Reducing initial page height

---

## 🎭 Theme Adaptation

### Dark Mode Colors
```css
background: #0d1117
surface: #1e1e1e
primary-text: #c9d1d9
accent: #355E3B
```

### Light Mode Colors
```css
background: #ffffff
surface: #f6f8fa
primary-text: #000000
accent: #355E3B
```

### Theme-Adaptive Images
```markdown
<picture>
  <source 
    media="(prefers-color-scheme: dark)" 
    srcset="dark-version.png">
  <source 
    media="(prefers-color-scheme: light)" 
    srcset="light-version.png">
  <img alt="Description" src="default.png" />
</picture>
```

---

## ♿ Accessibility Standards

### Color Contrast Ratios (WCAG AA)

| Text Size | Minimum Ratio | Example |
|-----------|---------------|---------|
| **Normal Text** (<18px) | 4.5:1 | #355E3B on #ffffff |
| **Large Text** (≥18px or bold 14px) | 3:1 | #355E3B on #f6f8fa |
| **UI Components** | 3:1 | Badges, buttons |

### Test Your Colors
```
Tool: https://webaim.org/resources/contrastchecker/

Example:
Foreground: #355E3B (Hunter Green)
Background: #ffffff (White)
Result: 7.5:1 (Pass AAA)
```

### Alt Text Guidelines

```markdown
<!-- Good Alt Text -->
![StrayDog Syndications LLC logo featuring hunter green branding]

<!-- Bad Alt Text -->
![Logo] or ![image]
```

**Alt Text Formula:**
1. Describe the content
2. Include context if relevant
3. Keep under 125 characters
4. Don't say "image of" or "picture of"

---

## 📊 API Configuration

### GitHub Stats API Parameters

| Parameter | Type | Options | Default |
|-----------|------|---------|---------|
| `username` | string | GitHub username | required |
| `theme` | string | dark, light, etc. | default |
| `show_icons` | boolean | true, false | true |
| `hide_border` | boolean | true, false | false |
| `include_all_commits` | boolean | true, false | false |
| `count_private` | boolean | true, false | false |
| `bg_color` | hex | Any hex (no #) | transparent |
| `title_color` | hex | Any hex (no #) | theme default |
| `icon_color` | hex | Any hex (no #) | theme default |
| `text_color` | hex | Any hex (no #) | theme default |

### Recommended Configurations

#### Dark Mode Optimal
```
?theme=dark
&bg_color=0d1117
&title_color=355E3B
&icon_color=355E3B
&text_color=c9d1d9
&hide_border=true
```

#### Light Mode Optimal
```
?theme=default
&title_color=355E3B
&icon_color=355E3B
&hide_border=true
```

---

## 🔢 Component Specifications

### Section Header
```markdown
---

## 🎯 Section Title

Content starts here...
```

**Specs:**
- H2 heading
- Emoji or icon prefix (optional)
- Horizontal rule above
- 2-3 line breaks after

### Badge Group
```markdown
<div align="center">

![Badge1] ![Badge2] ![Badge3]

</div>
```

**Specs:**
- Centered container
- Badges separated by spaces
- Related badges grouped
- Max 5-7 badges per row

### Project Card
```markdown
### Project Title

[![Live Demo](badge)](url) [![Source](badge)](url)

Description paragraph with key points.

**Technologies:** Tech1 · Tech2 · Tech3

**Key Features:** Feature1 · Feature2 · Feature3

---
```

**Specs:**
- H3 heading
- Action badges first
- One paragraph description
- Technologies bullet-separated with ·
- Features bullet-separated with ·
- Horizontal rule after

---

## 🎨 Visual Hierarchy

### Information Priority

**Primary (Largest/Bold):**
- Your name
- Current role/status
- Main sections

**Secondary (Medium):**
- Section descriptions
- Project titles
- Key statistics

**Tertiary (Regular):**
- Body text
- Lists
- Metadata

**Quaternary (Small/Muted):**
- Captions
- Timestamps
- Footer info

### Visual Weight Distribution

```
Header Section (20%)
├── Logo/Name
├── Title/Role
└── Social Links

Main Content (60%)
├── Professional Summary
├── Projects
├── Tech Stack
└── Experience

Stats & Metrics (15%)
├── GitHub Stats
├── Coding Platforms
└── Activity Graph

Footer (5%)
├── Contact CTA
└── Copyright
```

---

## 🛠️ Design Tokens Reference

### Quick Copy-Paste Values

#### Brand Color (Hunter Green)
```
Hex: #355E3B
RGB: rgb(53, 94, 59)
HSL: hsl(129, 28%, 29%)
RGBA: rgba(53, 94, 59, 1)
```

#### Spacing Scale
```
xs: 4px
sm: 8px
md: 16px
lg: 24px
xl: 32px
2xl: 48px
3xl: 64px
```

#### Border Radius
```
none: 0
sm: 2px
md: 4px
lg: 8px
full: 50% (circle)
```

#### Shadow Scale
```
sm: 0 1px 2px rgba(0,0,0,0.05)
md: 0 4px 6px rgba(0,0,0,0.1)
lg: 0 10px 15px rgba(0,0,0,0.1)
xl: 0 20px 25px rgba(0,0,0,0.15)
```

---

## 📱 Responsive Breakpoints

### Device Categories

| Device | Width Range | Layout Strategy |
|--------|-------------|-----------------|
| **Mobile** | < 768px | Single column, stacked |
| **Tablet** | 768px - 1024px | Two column where possible |
| **Desktop** | 1024px - 1440px | Full multi-column |
| **Large Desktop** | > 1440px | Optimized spacing |

### Testing Devices

**Priority Devices:**
- iPhone 12/13 Pro (390px)
- iPad (768px)
- MacBook Pro 13" (1440px)
- Desktop 1080p (1920px)

**Test Using:**
- Chrome DevTools responsive mode
- Actual devices
- GitHub mobile app
- Browser zoom levels (50%, 100%, 150%)

---

## ✅ Design Checklist

### Before Publishing

**Visual**
- [ ] Colors consistent with brand
- [ ] Contrast ratios meet WCAG AA
- [ ] Images optimized and compressed
- [ ] Badges render correctly
- [ ] Layout balanced and professional

**Typography**
- [ ] Heading hierarchy logical
- [ ] No orphaned headings
- [ ] Consistent font usage
- [ ] Readable line lengths
- [ ] Proper emphasis (bold/italic)

**Spacing**
- [ ] Consistent section breaks
- [ ] Adequate white space
- [ ] Aligned elements
- [ ] No awkward gaps
- [ ] Visual rhythm maintained

**Responsive**
- [ ] Mobile layout tested
- [ ] Tablet layout verified
- [ ] Desktop optimized
- [ ] No horizontal scrolling
- [ ] Touch targets adequate (44x44px)

**Accessibility**
- [ ] Alt text on all images
- [ ] Proper heading structure
- [ ] Sufficient contrast
- [ ] Descriptive links
- [ ] Keyboard navigable

---

## 🎯 Brand Guidelines Summary

### Core Principles

1. **Authentic**: Real achievements, honest representation
2. **Professional**: Clean, modern, industry-standard
3. **Mission-Driven**: Justice reform context evident
4. **Technical**: Demonstrates actual expertise
5. **Approachable**: Not intimidating, human

### Visual Language

**Colors**: Hunter Green dominance, semantic accents  
**Typography**: Clear hierarchy, readable  
**Layout**: Balanced, organized, scannable  
**Imagery**: Professional, relevant, optimized  
**Tone**: Confident but humble, technical but accessible

### Consistency Across Properties

- Use same Hunter Green (#355E3B) everywhere
- Maintain similar badge styles
- Keep heading hierarchy consistent
- Use same fonts where possible
- Apply same spacing principles

---

## 📚 Resources

### Design Tools
- [Shields.io Badge Generator](https://shields.io/)
- [Simple Icons Library](https://simpleicons.org/)
- [Color Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Image Optimizer](https://tinypng.com/)

### GitHub-Specific
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Markdown Guide](https://www.markdownguide.org/)
- [GFM Spec](https://github.github.com/gfm/)

### Inspiration
- [Awesome GitHub Profiles](https://github.com/abhisheknaiidu/awesome-github-profile-readme)

---

**This design system ensures consistency across your GitHub profile and can be extended to all StrayDog Syndications properties for unified branding.**

---

*Design System v1.0.0 | Last Updated: November 2025*
