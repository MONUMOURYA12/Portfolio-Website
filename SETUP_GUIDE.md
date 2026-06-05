# Portfolio Setup Guide

## Quick Start

### 1. Install Dependencies
```bash
cd c:\Users\monup\Todo\Portfolio
npm install
```

### 2. Run Development Server
```bash
npm run dev
```
The portfolio will be available at `http://localhost:5173`

---

## Customization Checklist

### 📝 Personal Information

**Navigation.jsx** - Line ~35
```jsx
<button className="nav-btn btn btn-primary">Download CV</button>
```
- Update "Download CV" button with link to your CV

**Hero.jsx** - Update headline and subtitle
- Change "Hi, I'm a Full Stack Developer" to your introduction
- Update the subtitle with your focus areas
- Adjust stats (5+ Projects, 2+ Years Experience, 100% Satisfaction)

**About.jsx** - Update:
- "Who Am I?" section text
- Experience list (update years and technologies)
- Education section
- Skills and certifications

**Contact.jsx** - Update:
- Email: `your.email@example.com`
- Phone: `+1 (234) 567-890`
- Location: `Your City, Country`
- Social media links (GitHub, LinkedIn, Twitter)

**Footer.jsx** - Update:
- `Your Name` in copyright text
- Footer section links if needed

---

### 🎨 Projects

**Projects.jsx** - Update the `projects` array:

```javascript
{
  id: 1,
  title: 'Your Project Name',
  description: 'Project description here',
  technologies: ['React', 'Node.js', 'MongoDB'],
  features: ['Feature 1', 'Feature 2', 'Feature 3'],
  link: 'https://live-project-url.com',
  github: 'https://github.com/username/repo',
  image: '📝', // Use emoji or update to use actual images
  status: 'Completed' // or 'In Progress'
}
```

---

### 💻 Skills

**Skills.jsx** - Update the `skillCategories` array:

```javascript
{
  name: 'Frontend',
  skills: ['React', 'JavaScript/ES6+', 'HTML5', 'CSS3', ...]
}
```

Update proficiency levels in the proficiency section (modify width values: 90%, 85%, etc.)

---

### 🎨 Theme Customization

Edit `src/index.css` CSS variables:

```css
:root {
  --primary-color: #2563eb;        /* Main color */
  --secondary-color: #1e40af;      /* Hover/secondary */
  --accent-color: #f59e0b;         /* Highlights */
  --text-dark: #1f2937;
  --text-light: #6b7280;
  --bg-light: #f9fafb;
  --bg-white: #ffffff;
  --border-color: #e5e7eb;
}
```

Popular color schemes:
- **Modern Blue**: Primary: #2563eb, Secondary: #1e40af, Accent: #f59e0b
- **Tech Purple**: Primary: #7c3aed, Secondary: #6d28d9, Accent: #ec4899
- **Fresh Green**: Primary: #10b981, Secondary: #059669, Accent: #f59e0b
- **Dark Mode**: Primary: #60a5fa, Secondary: #3b82f6, Accent: #fbbf24

---

### 📦 Build & Deploy

**Build for Production:**
```bash
npm run build
```
This creates a `dist` folder with optimized files.

**Preview Production Build:**
```bash
npm run preview
```

**Deploy Options:**

1. **Vercel** (Recommended)
   - Push to GitHub
   - Import repo in Vercel
   - Auto-deploy on push

2. **Netlify**
   - Push to GitHub
   - Connect via Netlify
   - Set build: `npm run build`, publish: `dist`

3. **GitHub Pages**
   - Update `vite.config.js` with `base: '/repo-name/'`
   - Push to `gh-pages` branch

---

### 📱 Image Handling

Currently using emojis for project images (📝, 🛒, 📊, etc.)

To use real images:
1. Add images to `public/images/` folder
2. Update Projects.jsx:
```jsx
image: require('../../public/images/project1.jpg')
// or use direct path
image: '/images/project1.jpg'
```
3. Update component to use `<img src={project.image} />`

---

### 🔍 SEO Optimization

1. Update `index.html` title and meta tags
2. Add meta descriptions
3. Use semantic HTML (already done)
4. Consider adding `robots.txt` and `sitemap.xml` before deployment

---

### 📋 Components Structure

```
src/components/
├── Navigation.jsx    - Navbar with smooth scrolling
├── Hero.jsx          - Landing section with CTA
├── About.jsx         - About section with experience
├── Projects.jsx      - Project showcase grid
├── Skills.jsx        - Skills and proficiency levels
├── Contact.jsx       - Contact form + info
└── Footer.jsx        - Footer with links
```

---

## Tips for Success

✅ **Do:**
- Keep descriptions concise and impactful
- Use real project links when available
- Regularly update projects and skills
- Test on mobile devices
- Optimize images before adding

❌ **Don't:**
- Leave placeholder text (update all sections)
- Use broken links
- Forget to add your actual contact info
- Ignore mobile responsiveness

---

## Common Customizations

### Change Primary Color
In `src/index.css`, change `--primary-color` to your preferred color

### Add More Projects
Add objects to the `projects` array in `Projects.jsx`

### Modify Font
Update `font-family` in `src/index.css` body style

### Add Resume/CV
Add a download button in Navigation.jsx pointing to your CV file

### Enable Contact Form
Replace console.log in Contact.jsx with actual backend/service (Emailjs, Formspree, etc.)

---

## Questions?

Refer to component files for detailed comments and structure.
Good luck with your portfolio! 🚀
