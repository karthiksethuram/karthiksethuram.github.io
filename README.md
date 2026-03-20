# Karthikeyan Sethuraman - Data Scientist Portfolio

A professional, modern portfolio website showcasing 10+ years of data science and machine learning expertise across healthcare, finance, retail, and enterprise domains.

## 🎯 Features

- **Responsive Design** - Works seamlessly on mobile, tablet, and desktop devices
- **Modern Aesthetic** - Clean, professional design with deep slate blue and vibrant teal accents
- **Project Showcase** - Interactive project cards with technology filtering
- **Experience Timeline** - Visual timeline of professional roles and achievements
- **Skills Organization** - Categorized technical skills (Languages, ML/AI, Analytics, Databases, Tools)
- **Education Section** - Degrees, coursework, and academic achievements
- **Contact Integration** - Direct links to email, LinkedIn, and GitHub
- **Smooth Interactions** - Hover effects, transitions, and animations throughout

## 🏗️ Project Structure

```
portfolio-website/
├── client/
│   ├── public/              # Static files (favicon, robots.txt)
│   ├── src/
│   │   ├── components/      # Reusable React components
│   │   │   ├── ProjectCard.tsx
│   │   │   ├── ExperienceCard.tsx
│   │   │   └── ...
│   │   ├── pages/           # Page components
│   │   │   └── Home.tsx
│   │   ├── data/            # Portfolio content
│   │   │   └── portfolio.ts
│   │   ├── contexts/        # React contexts (Theme)
│   │   ├── App.tsx          # Main app component
│   │   ├── main.tsx         # React entry point
│   │   └── index.css        # Global styles and design tokens
│   └── index.html           # HTML template
├── server/                  # Express server (static deployment)
├── package.json             # Dependencies and scripts
├── DEPLOYMENT_GUIDE.md      # GitHub Pages deployment instructions
├── PORTFOLIO_STRUCTURE.md   # Content architecture and data model
└── ideas.md                 # Design philosophy and approach
```

## 🎨 Design System

### Color Palette
- **Primary**: Deep Slate Blue (#1e293b) - Authority and tech credibility
- **Accent**: Vibrant Teal (#06b6d4) - Interactive elements and highlights
- **Background**: Off-white (#f8fafc) - Clean, professional backdrop
- **Neutral**: Gray scale (#e2e8f0 to #64748b) - Supporting text and borders

### Typography
- **Headings**: Poppins Bold (700) - Strong visual hierarchy
- **Body**: Inter Regular (400) - Readable, professional
- **Labels**: Inter Medium (500) - Emphasis and tags

### Spacing
- Base unit: 1.5rem (24px)
- Generous whitespace for clarity and breathing room
- Responsive padding adjustments for mobile/tablet/desktop

## 📝 Content Management

All portfolio content is stored in a single TypeScript file for easy updates:

**File**: `client/src/data/portfolio.ts`

### Adding a New Project

```typescript
{
  id: "2",
  title: "Your Project Title",
  description: "2-3 sentence description of the project",
  technologies: ["Python", "Machine Learning", "Data Analysis"],
  keyResults: ["Key achievement 1", "Key achievement 2"],
  category: "Machine Learning",
  date: "2024-03",
  featured: true,
}
```

### Adding a New Experience Entry

```typescript
{
  id: "7",
  company: "Company Name",
  jobTitle: "Your Job Title",
  location: "City, Country",
  startDate: "2024-01",
  endDate: "Present",
  description: ["Achievement 1", "Achievement 2"],
  technologies: ["Python", "SQL", "Analytics"],
}
```

### Updating Skills

Skills are organized by category in the `skills` object:
- `languages` - Programming languages
- `mlAi` - Machine learning and AI techniques
- `analytics` - Analytics and modeling approaches
- `databases` - Database technologies
- `tools` - Tools and platforms

## 🚀 Getting Started

### Local Development

1. **Install dependencies**:
   ```bash
   cd portfolio-website
   npm install
   ```

2. **Start development server**:
   ```bash
   npm run dev
   ```
   The site will be available at `http://localhost:3000`

3. **Build for production**:
   ```bash
   npm run build
   ```

### Deployment to GitHub Pages

See `DEPLOYMENT_GUIDE.md` for detailed instructions on deploying to GitHub Pages.

## 🔧 Customization

### Changing Colors

Edit the CSS variables in `client/src/index.css`:

```css
:root {
  --primary: #1e293b;        /* Deep Slate Blue */
  --accent: #06b6d4;         /* Vibrant Teal */
  --background: #f8fafc;     /* Off-white */
  /* ... more colors ... */
}
```

### Modifying Fonts

Update the Google Fonts import in `client/src/index.css`:

```css
@import url('https://fonts.googleapis.com/css2?family=YOUR_FONT:wght@400;500;600;700&display=swap');
```

### Adding New Sections

1. Create a new component in `client/src/components/`
2. Import and use it in `client/src/pages/Home.tsx`
3. Add corresponding data to `client/src/data/portfolio.ts`

## 📱 Responsive Breakpoints

- **Mobile**: < 640px - Single column layout
- **Tablet**: 640px - 1024px - 2-column grid
- **Desktop**: > 1024px - 3-column grid with sidebar

## ♿ Accessibility

- Semantic HTML structure
- ARIA labels for interactive elements
- Keyboard navigation support
- High contrast text for readability
- Focus indicators on interactive elements

## 🔄 Future Enhancements

Consider adding:

1. **Dark Mode Toggle** - Uncomment `switchable` in `App.tsx`
2. **Blog Section** - Technical articles and insights
3. **Case Studies** - Detailed project breakdowns
4. **Analytics** - Track visitor engagement
5. **Search Functionality** - Find projects by keyword
6. **Comments Section** - Engage with visitors
7. **Newsletter Signup** - Build audience

## 📚 Technologies Used

- **React 19** - UI framework
- **TypeScript** - Type safety
- **Tailwind CSS 4** - Utility-first styling
- **shadcn/ui** - Component library
- **Vite** - Build tool
- **Wouter** - Client-side routing
- **Lucide React** - Icons

## 📄 License

This portfolio website is open source and available under the MIT License.

## 👤 Author

**Karthikeyan Sethuraman**
- Email: ksethuramam1992@gmail.com
- LinkedIn: [linkedin.com/in/karthikeyan-sethuraman/](https://www.linkedin.com/in/karthikeyan-sethuraman/)
- GitHub: [github.com/karthiksethuram](https://github.com/karthiksethuram)
- Location: Plano, TX

## 🤝 Support

For issues, questions, or suggestions, please reach out via email or LinkedIn.

---

**Last Updated**: March 2024
**Version**: 1.0.0
