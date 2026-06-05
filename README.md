# Full Stack Developer Portfolio

A modern, responsive portfolio website built with React and Vite, showcasing projects, skills, and experience.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Projects Showcase**: Display your best projects with descriptions and technologies
- **Skills Section**: Highlight your technical expertise with proficiency levels
- **Contact Form**: Easy way for potential clients/employers to reach you
- **Navigation**: Smooth scrolling navigation to different sections

## Project Sections

1. **Hero/Landing** - Eye-catching introduction with call-to-action buttons
2. **About** - Personal summary and key highlights
3. **Projects** - Showcase of 6 featured projects with full details
4. **Skills** - Categorized skills and proficiency levels
5. **Contact** - Contact form and methods to reach you

## Tech Stack

- **Frontend**: React 19
- **Build Tool**: Vite 8
- **Styling**: CSS3
- **Linting**: ESLint

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build for production
- `npm run preview` - Preview the production build
- `npm run lint` - Run ESLint to check code quality

## Customization

### Update Personal Information

Edit the following sections to match your information:

1. **Navigation.jsx** - Logo and navigation menu
2. **Hero.jsx** - Hero section content
3. **About.jsx** - About section and personal details
4. **Projects.jsx** - Update the `projects` array with your projects
5. **Skills.jsx** - Update the `skillCategories` array with your skills
6. **Contact.jsx** - Update email, phone, and social links

### Modify Colors

Edit the CSS variables in `index.css`:

```css
:root {
  --primary-color: #2563eb;
  --secondary-color: #1e40af;
  --accent-color: #f59e0b;
  /* ... other colors ... */
}
```

## File Structure

```
Portfolio/
├── public/
├── src/
│   ├── components/
│   │   ├── Navigation.jsx
│   │   ├── Hero.jsx
│   │   ├── About.jsx
│   │   ├── Projects.jsx
│   │   ├── Skills.jsx
│   │   ├── Contact.jsx
│   │   ├── Footer.jsx
│   │   └── *.css
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── index.html
├── package.json
├── vite.config.js
├── eslint.config.js
└── README.md
```

## Deployment

### Deploy to Vercel

1. Push your code to GitHub
2. Go to [Vercel](https://vercel.com)
3. Click "New Project" and import your repository
4. Vercel will automatically detect Vite and configure the build settings
5. Click "Deploy"

### Deploy to Netlify

1. Push your code to GitHub
2. Go to [Netlify](https://netlify.com)
3. Click "New site from Git"
4. Select your repository
5. Set build command to `npm run build` and publish directory to `dist`
6. Click "Deploy"

## Performance Tips

- Optimize images before adding them to the portfolio
- Use CSS minification in production builds (automatic with Vite)
- Consider lazy loading for project images
- Use semantic HTML for better SEO

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This project is open source and available under the MIT License.

## Contact

For questions or inquiries about this portfolio template, feel free to reach out.

---

**Made with ❤️ for developers**
