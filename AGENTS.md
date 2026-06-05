# AI Agent Customization Guide for Curriculum_Vitae Project

## Project Overview
This is a **curriculum vitae (CV) and resume repository** containing multiple versions of Renato de Bakker's professional profile in different formats, languages, and design templates. It serves as both a portfolio showcase and a learning project for web development.

## Key Project Files

### CV Source Files
- **`RenatoCV.md`** - Primary markdown source with content structure (Name, Email, Summary, Skills)
- **`RenatoCV.txt`** - Plain text version of the CV
- **HTML Templates** - Multiple styled versions:
  - `index.html` - Main portfolio page
  - `My_CV.html`, `my-cv.html` - English CV with professional styling
  - `Resume.html` - Resume format
  - `cafeCV.html`, `data-analysis.html`, `zaaCV.html` - Alternative template designs
  - `German-My_CV.html`, `Lebenslauf.html` - German language versions

### Assets
- `Renato_image.png` - Profile picture referenced in CV files
- `README.md` - Minimal project README

## Development Conventions

### Content Management
1. **Single Source of Truth**: Update `RenatoCV.md` first, then propagate changes to other formats
2. **Format Consistency**: Maintain the same structure across all versions:
   - Personal Information (Name, Email, Phone if applicable)
   - Professional Summary
   - Programming Languages
   - Web Development Skills
   - Tools & Software
   - Soft Skills
   - Additional Skills/Certifications

### HTML Templates
- Uses **Font Awesome icons** via CDN (`cdnjs.cloudflare.com`)
- Common CSS patterns:
  - Gradient backgrounds (#4b6cb7 to #182848 blue theme)
  - A4 paper sizing for print compatibility (`210mm × 297mm`)
  - Responsive flex layouts with `max-width: 1000px` or `210mm`
  - Box shadows for depth: `0 5px 15px rgba(0, 0, 0, 0.1)`

### Language & Localization
- **English**: Primary language (My_CV.html, Resume.html, etc.)
- **German**: Lebenslauf.html (German for "CV/Résumé")
- Naming follows pattern: `[Type]-[Language]-CV.html` or `[Type]CV.html`

## Common Tasks for AI Agents

### Task: Update CV Content
1. Edit `RenatoCV.md` with new information
2. Update corresponding HTML files (search for old content, replace with new)
3. Maintain semantic HTML structure (`<header>`, `<section>`, proper heading hierarchy)
4. Ensure image path references work correctly

### Task: Create New CV Template
1. Use existing template as base (e.g., `My_CV.html`)
2. Keep the same CSS structure (gradients, spacing, A4 sizing)
3. Add file to naming convention: `[descriptive]-CV.html`
4. Include Font Awesome icon references for visual consistency
5. Test responsive design on mobile (meta viewport already set)

### Task: Add Skills or Sections
1. Add to `RenatoCV.md` first
2. Update all HTML versions consistently
3. Use semantic HTML: `<section>` for major sections, `<ul>` for lists
4. Maintain visual hierarchy with consistent spacing and colors

## Technical Stack
- **Frontend**: HTML5, CSS3 (Flexbox/Grid)
- **Styling**: Inline CSS in HTML files (no external stylesheet)
- **Icons**: Font Awesome 6.4.0 (CDN)
- **Version Control**: Git repo present (`.git/` directory)
- **Content Formats**: HTML, Markdown (.md), Plain Text (.txt)

## Important Notes for AI Agents

1. **Print Compatibility**: HTML files use `@media print` rules and A4 dimensions. Test print preview when modifying styles.
2. **Image Assets**: Profile image path is `Renato_image.png` - verify it exists before referencing in new templates.
3. **CDN Dependencies**: Font Awesome icons load from CDN. Test that styles render correctly.
4. **Multi-file Updates**: CV content changes typically require updating multiple HTML files - coordinate these together.
5. **Empty Directory**: `bubble-sort/` folder exists but is empty (likely a placeholder for future projects).

## Suggested Next Customizations

- **Skill: CV Content Migration** - Automate updating all HTML files when `RenatoCV.md` changes
- **Skill: Template Generator** - Quick scaffolding for new CV template variations
