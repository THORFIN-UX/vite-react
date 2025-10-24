# Anir Kesstaou - Portfolio Website

A modern, elegant, and fully responsive portfolio website built with React, TypeScript, Tailwind CSS, and Framer Motion.

## Features

- **Modern Design**: Clean, futuristic aesthetic with subtle 3D effects and smooth animations
- **Dark Mode**: Default dark theme with persistent light/dark mode toggle
- **Fully Responsive**: Mobile-first design optimized for all screen sizes
- **Performance Optimized**: Fast loading times and smooth interactions
- **SEO Ready**: Comprehensive meta tags, Open Graph, and JSON-LD schema
- **Accessibility**: Semantic HTML, keyboard navigation, and ARIA labels
- **Easy to Customize**: Well-organized code structure with clear configuration files

## Tech Stack

- **React 18+** - Modern UI library with hooks
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first styling
- **Framer Motion** - Smooth animations and transitions
- **Vite** - Fast build tool and dev server
- **Lucide React** - Beautiful icon set

## Getting Started

### Prerequisites

- Node.js 18+ and npm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/anirkesstaou/portfolio.git
cd portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:5173`

## Customization Guide

### Personal Information

Update your personal details in the following locations:

#### 1. Meta Tags and SEO (`index.html`)
```html
<title>Your Name - Web Developer | Portfolio</title>
<meta name="description" content="Your description here" />
<meta name="author" content="Your Name" />
<meta property="og:url" content="https://yourdomain.com" />
```

#### 2. Hero Section (`src/components/Hero.tsx`)
```typescript
<h1>Your Name</h1>
<h2>Your Title</h2>
<p>Your tagline here</p>
```

#### 3. Footer (`src/components/Footer.tsx`)
```typescript
<span>© {currentYear} Your Name</span>
```

### Projects

Edit your projects in `src/data/projects.ts`:

```typescript
export const projects: Project[] = [
  {
    id: 1,
    title: 'Project Title',
    description: 'Project description',
    technologies: ['React', 'TypeScript', 'etc'],
    link: 'https://project-link.com',
    github: 'https://github.com/username/repo'
  },
  // Add more projects...
];
```

### Skills

Update your skills in `src/components/Skills.tsx`:

```typescript
const skillCategories: SkillCategory[] = [
  {
    title: 'Category Name',
    skills: ['Skill 1', 'Skill 2', 'Skill 3'],
    color: 'from-accent-primary to-accent-primary/70'
  },
  // Add more categories...
];
```

### Contact Links

Modify social links in `src/components/Contact.tsx`:

```typescript
const socialLinks = [
  {
    name: 'Email',
    icon: Mail,
    href: 'mailto:your@email.com',
    label: 'your@email.com',
    color: 'hover:text-accent-primary'
  },
  // Update with your links...
];
```

### About Section

Edit the about text in `src/components/About.tsx`:

```typescript
<p>Your introduction text here...</p>
```

### Theme Colors

Customize colors in `tailwind.config.js`:

```javascript
colors: {
  accent: {
    primary: '#3b82f6',    // Change to your brand color
    secondary: '#8b5cf6',  // Change to your secondary color
    tertiary: '#06b6d4',   // Change to your tertiary color
  },
}
```

## Building for Production

Create an optimized production build:

```bash
npm run build
```

The build output will be in the `dist` directory.

## Deployment

### Vercel

1. Push your code to GitHub
2. Import your repository in Vercel
3. Deploy with one click

### Netlify

1. Push your code to GitHub
2. Connect your repository in Netlify
3. Build command: `npm run build`
4. Publish directory: `dist`

### GitHub Pages

1. Install gh-pages:
```bash
npm install --save-dev gh-pages
```

2. Add to package.json:
```json
"homepage": "https://yourusername.github.io",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d dist"
}
```

3. Deploy:
```bash
npm run deploy
```

## Project Structure

```
src/
├── components/       # React components
│   ├── Navigation.tsx
│   ├── Hero.tsx
│   ├── About.tsx
│   ├── Skills.tsx
│   ├── Projects.tsx
│   ├── Contact.tsx
│   └── Footer.tsx
├── data/            # Data files
│   └── projects.ts  # Projects configuration
├── hooks/           # Custom React hooks
│   └── useTheme.ts  # Theme management
├── App.tsx          # Main app component
├── main.tsx         # App entry point
└── index.css        # Global styles
```

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run typecheck` - Run TypeScript type checking

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

MIT License - feel free to use this template for your own portfolio!

## Credits

Created by Anir Kesstaou

---

**Note**: Remember to update all placeholder links and content with your actual information before deploying!
