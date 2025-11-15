# Apollo Landing Page

A modern, responsive landing page for Apollo - Advanced Programming and Online Learning Laboratory. Built with HTML5, Tailwind CSS 4, and vanilla JavaScript.

## Features

- ✨ **Fully Responsive Design** - Mobile-first approach with breakpoints for all screen sizes
- 📱 **Mobile Burger Menu** - Animated hamburger menu with smooth sidebar navigation
- 🎨 **Modern UI** - Clean and professional design with Tailwind CSS
- 🔗 **Smooth Scroll Navigation** - Anchor links with smooth scrolling behavior
- ⚡ **Lightweight** - No heavy dependencies, uses vanilla JavaScript
- 🎯 **Blur Overlay Effect** - Beautiful backdrop blur effect on mobile sidebar
- 📦 **Pre-configured** - All dependencies and configurations are ready to use

## Project Structure

```
apollo-landing-page/
├── index.html           # Main HTML file
├── package.json         # Project dependencies
├── package-lock.json    # Lock file for dependencies
├── .gitignore          # Git ignore configuration
├── README.md           # This file
├── src/
│   ├── input.css       # Tailwind CSS input
│   └── output.css      # Compiled CSS (auto-generated)
└── assets/             # Image assets
    ├── logo-header.svg
    ├── logo-footer.svg
    ├── ilustation.svg
    ├── globe.svg
    ├── code.svg
    ├── portofolio.svg
    ├── RoketCTA.svg
    └── ... (other assets)
```

## Getting Started

### Prerequisites

- **Node.js** (v14 or higher)
- **npm** (comes with Node.js)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yudha556/Apollo-landing-page.git
   cd Apollo-landing-page
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Build CSS (if needed)**
   ```bash
   npm run build
   ```

4. **Start development mode** (auto-compile CSS on file changes)
   ```bash
   npm run dev
   ```

## Available Scripts

### `npm run build`
Compiles the Tailwind CSS from `src/input.css` to `src/output.css`. Run this after making changes if not in watch mode.

```bash
npm run build
```

### `npm run dev`
Starts the Tailwind CLI in watch mode, automatically recompiling CSS whenever you modify your HTML or CSS files.

```bash
npm run dev
```

## Technologies Used

- **HTML5** - Semantic markup and structure
- **Tailwind CSS 4** - Utility-first CSS framework
- **Tailwind CLI** - Command-line tool for building CSS
- **JavaScript (Vanilla)** - Interactive features and smooth scroll navigation

## How to Use

### Viewing the Website

Open `index.html` directly in your browser or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using VS Code Live Server
# Install "Live Server" extension and click "Go Live"
```

Then navigate to `http://localhost:8000` (or the port shown in terminal).

### Customizing the Design

1. **Colors** - Modify Tailwind color classes in `index.html`
2. **Content** - Edit text and images directly in `index.html`
3. **Styles** - Add custom CSS in `src/input.css` for custom styles
4. **Rebuild** - After changes, the CSS will auto-compile if you're in dev mode

### Mobile Responsive Breakpoints

The design uses Tailwind's responsive prefixes:
- `md:` - Medium screens and up (768px+)
- Mobile styles are default, desktop styles use `md:` prefix

Example:
```html
<div class="px-6 md:px-16">  <!-- 6 on mobile, 16 on desktop -->
  <h1 class="text-3xl md:text-5xl">Responsive Heading</h1>
</div>
```

## Navigation Sections

The page has the following scroll sections:

1. **Header** - Navigation bar with burger menu
2. **Home** (`#home`) - Hero section with main call-to-action
3. **Features** (`#features`) - Three feature cards
4. **CTA** (`#cta`) - Call-to-action section
5. **Footer** - Contact and quick links

You can navigate between sections using the navigation menu or smooth scroll links.

## JavaScript Features

### Burger Menu
- Click the hamburger icon to toggle mobile sidebar
- Click overlay or close button to close sidebar
- Menu automatically closes when navigation link is clicked
- Animated burger lines transform to X when opened

### Smooth Scroll
- Click any navigation link to smoothly scroll to section
- Implemented with vanilla JavaScript `scrollIntoView()` API
- Works on both desktop navigation and mobile sidebar

## File Configuration

### package.json
Contains project metadata and scripts for building CSS:
- `tailwindcss` - CSS framework
- `@tailwindcss/cli` - CLI tool for building CSS

### .gitignore
Configured to exclude:
- `node_modules/` - Dependencies (install locally with npm install)
- Environment variables
- IDE files
- OS files

## Contributing

When contributing:

1. Keep the responsive design intact
2. Test on both mobile and desktop views
3. Follow the existing code style
4. Update CSS using `src/input.css` for custom styles
5. Run `npm run build` before committing

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Troubleshooting

### CSS not updating?
- Make sure `src/output.css` is linked in `index.html`
- Run `npm run build` to recompile CSS
- Clear browser cache (Ctrl+Shift+Delete)

### Burger menu not working?
- Check browser console for JavaScript errors (F12)
- Verify IDs in HTML match JavaScript selectors

### Dependencies installation fails?
- Delete `node_modules` and `package-lock.json`
- Run `npm cache clean --force`
- Run `npm install` again

## License

This project is open source and available under the MIT License.

## Author

Created by Yudha (yudha556)

---

**Happy coding!** If you have any questions or issues, feel free to open an issue on the repository.
