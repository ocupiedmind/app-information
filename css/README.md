# CSS Styles Documentation

This folder contains the styling for the App Privacy Policy Hub website.

## Files

- **`styles.css`** - Compiled CSS file with all styles
- **`styles.scss`** - SASS source file with variables, mixins, and nested selectors
- **`README.md`** - This documentation file

## Structure

### CSS Custom Properties (Variables)
All colors, shadows, and common values are defined as CSS custom properties for easy theming:

```css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    --text-color: #2c3e50;
    --light-bg: #f8f9fa;
    --card-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    --hover-shadow: 0 8px 15px rgba(0, 0, 0, 0.15);
    --border-color: #e9ecef;
}
```

### SASS Features
The SASS version includes:

- **Variables**: Color schemes, shadows, gradients
- **Mixins**: 
  - `@mixin glassmorphism` - Glass effect styling
  - `@mixin gradient-text()` - Gradient text effects
  - `@mixin hover-lift` - Hover animations
  - `@mixin responsive()` - Media query helpers
- **Nested Selectors**: Organized, maintainable CSS structure

### Component Organization

#### Index Page Styles
- `.hero-section` - Main title and subtitle area
- `.policy-card` - Individual privacy policy cards
- `.footer` - Site footer with contact information

#### Privacy Policy Page Styles
- `.privacy-content` - Main content container
- `.header-section` - Page title and effective date
- `.section-title` - Section headings with icons
- `.contact-section` - Contact information highlight
- `.back-button` - Navigation back to hub

### Responsive Design
Mobile-first responsive design with breakpoints at 768px for:
- Font size adjustments
- Padding and margin changes
- Layout modifications
- Button positioning

### Browser Support
- Modern browsers with CSS Grid and Flexbox support
- Backdrop-filter for glassmorphism effects
- CSS custom properties (CSS variables)
- Gradient text effects

## Usage

1. **For development**: Edit `styles.scss` and compile to CSS
2. **For production**: Use the compiled `styles.css` file
3. **For customization**: Modify CSS custom properties in `:root`

## Compilation

To compile SASS to CSS:
```bash
sass css/styles.scss css/styles.css
```

For development with watch mode:
```bash
sass --watch css/styles.scss css/styles.css
```
