# Reliability, Resilience and Incident Management

> A comprehensive presentation on operational excellence and high-performance operations by Andrew Hatch (@hatchman76)

## 📖 About This Presentation

This presentation covers essential principles and practices for building reliable, resilient systems and managing incidents effectively. It's designed for engineering teams, SREs, platform engineers, and anyone involved in operational excellence.

### 🎯 Core Topics Covered

- **Alerting** - Best practices for meaningful, actionable alerts
- **Metrics** - Building metrics that tell stories and drive decisions  
- **Monitoring** - Customer-focused observability strategies
- **Deployment Safety** - Progressive rollouts, canaries, and automation
- **Incidents & On-Call** - Learning from incidents and sustainable on-call practices
- **Discipline & Ritual** - Operational hygiene and continuous improvement

### 💡 Key Principles

- Customers are not your monitoring system
- Incidents are learning opportunities, not just interruptions
- New features should never compromise core experiences
- On-call is a core engineering discipline

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional, for best experience)

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/hatchman1976/mindvalley.git
   cd mindvalley
   ```

2. **Open the presentation:**
   
   **Option A: Direct file access**
   ```bash
   open src/index.htm
   # or double-click src/index.htm in your file manager
   ```
   
   **Option B: Local web server (recommended)**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx http-server
   
   # Using PHP
   php -S localhost:8000
   ```
   
   Then visit: `http://localhost:8000/src/index.htm`

### 🎮 Navigation Controls

| Key | Action |
|-----|--------|
| `Space` / `→` | Next slide |
| `←` | Previous slide |
| `Home` | First slide |
| `End` | Last slide |
| `Esc` | Overview mode |
| `?` | Help |

**Mouse/Touch:**
- Click to advance slides
- Use toolbar controls (bottom-right)
- Swipe on mobile devices

## 🏗️ Technical Architecture

### Built With

- **[Impress.js](https://impress.js.org/)** - 3D presentation framework
- **HTML5** - Semantic markup and structure
- **CSS3** - Styling, animations, and responsive design
- **JavaScript** - Interactive animations and controls
- **Google Fonts** - Typography (Courier Prime, Comic Sans MS)

### Key Features

- **🎨 3D Transitions** - Smooth camera movements between slides
- **📱 Responsive Design** - Works on desktop, tablet, and mobile
- **🎬 Slide Animations** - Substep animations for progressive reveals
- **📖 Book Showcase** - Animated book cover reveals with recommendations
- **🌍 Interactive Maps** - Visual storytelling for speaker background
- **📊 Rich Content** - Tables, images, and structured information
- **⚡ Fast Loading** - Optimized assets and efficient CSS
- **♿ Accessible** - Semantic HTML and keyboard navigation

### Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ⚠️ Internet Explorer not supported

## 📁 Project Structure

```
mindvalley/
├── README.md                 # This file
├── src/
│   ├── index.htm            # Main presentation file
│   ├── css/
│   │   ├── presentation.css # Main presentation styles
│   │   ├── fonts.css        # Font definitions
│   │   └── ...              # Additional CSS files
│   ├── images/              # All presentation images
│   │   ├── book-*.png       # Book cover images
│   │   ├── emoji-*.png      # Emoji icons
│   │   └── ...              # Maps, logos, photos
│   ├── js/
│   │   └── impress.js       # Core presentation engine
│   ├── lib/                 # Impress.js libraries
│   │   ├── gc.js            # Garbage collection
│   │   ├── rotation.js      # 3D rotation utilities
│   │   └── util.js          # Utility functions
│   └── plugins/             # Impress.js plugins
│       ├── autoplay/        # Auto-advance slides
│       ├── navigation/      # Keyboard/mouse navigation
│       ├── substep/         # Progressive reveals
│       └── ...              # Additional plugins
```

## 🎨 Customization Guide

### Modifying Content

1. **Edit slides:** Update content in `src/index.htm`
2. **Add images:** Place files in `src/images/` and reference in HTML
3. **Update styling:** Modify `src/css/presentation.css`
4. **Change fonts:** Update font imports in `src/css/fonts.css`

### Adding New Slides

```html
<!-- Add after existing slides in src/index.htm -->
<div id="stepN" class="step" data-x="X_POSITION" data-y="Y_POSITION" data-scale="SCALE">
    <h1>Your Slide Title</h1>
    <p>Your content here...</p>
</div>
```

### Slide Positioning

Slides are positioned in 3D space using data attributes:
- `data-x` / `data-y` - 2D position
- `data-z` - Depth (3D)
- `data-scale` - Zoom level
- `data-rotate-x/y/z` - 3D rotation

### Styling Guidelines

The presentation uses a clean, professional color scheme:
- **Background:** Light cream (`rgb(255, 243, 224)`)
- **Text:** Dark (`#000000`)
- **Accent:** Royal blue (`royalblue`)
- **Fonts:** Courier New (headings), Comic Sans MS (body)

## 📚 Content Sources & References

### Recommended Reading

The presentation references several influential books:
- [The Site Reliability Workbook](https://www.goodreads.com/book/show/39687146-the-site-reliability-workbook)
- [The DevOps Handbook](https://www.goodreads.com/book/show/26083308-the-devops-handbook)
- [Chaos Engineering](https://www.goodreads.com/book/show/45689179-chaos-engineering)
- [The Phoenix Project](https://www.goodreads.com/book/show/17255186-the-phoenix-project)
- [Field Guide to Human Error](https://www.goodreads.com/book/show/152014656-the-field-guide-to-understanding-human-error-3rd-edition-by-sidney-dek)
- And many more listed in the presentation

### Related Content

- 📺 [Confessions of an SRE Manager](https://youtu.be/y1rzaL_mOpM?si=n8S6qUb0Y_pqdIxc)
- 📺 [Learning from Incidents](https://youtu.be/TIL6UP9K-L4?si=ioigOpPBRQI3QS6d)
- 📺 [Learning more from Complex Systems](https://youtu.be/5pKGW61Ryvo?si=UDfRdaT0qdH3-OoY)
- 📝 [Medium Blog Series - Improving Incident Learning](https://medium.com/seek-blog/improving-incident-learning-part-1-d021362f1e6b)

## 🔧 Development & Maintenance

### File Organization

The codebase is organized with clear separation of concerns:
- **HTML:** Semantic structure with detailed comments
- **CSS:** Modular stylesheets with clear section headers
- **JavaScript:** Well-documented libraries and plugins
- **Assets:** Organized image directories with descriptive names

### Code Style

- 4-space indentation
- Semantic HTML5 elements
- BEM-style CSS naming where applicable
- Comprehensive comments and documentation
- Consistent formatting and spacing

### Performance Considerations

- Optimized image sizes
- Efficient CSS selectors
- Minimal JavaScript execution
- Local font files for offline usage
- Progressive loading of slide content

## 🌐 Deployment

### GitHub Pages

To deploy via GitHub Pages:

1. Push code to GitHub repository
2. Go to repository Settings → Pages
3. Select source branch (usually `main`)
4. Set folder to `/` (root)
5. Access at: `https://yourusername.github.io/mindvalley/src/index.htm`

### Other Hosting Options

- **Netlify:** Drag and drop the entire folder
- **Vercel:** Connect GitHub repository
- **AWS S3:** Upload to S3 bucket with static website hosting
- **Any web server:** Upload files and serve statically

## 🤝 Contributing

While this is a personal presentation, suggestions and improvements are welcome:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This presentation is available under the MIT License. The content reflects personal views and experiences in operational excellence and incident management.

## 👨‍💻 About the Author

**Andrew Hatch** (@hatchman76)
- SRE Manager with 15+ years in infrastructure
- Experience at LinkedIn, ThousandEyes, and across Australia/India/USA
- Passionate about operational excellence and learning from incidents
- 🔗 [LinkedIn](https://linkedin.com/in/hatchman76)
- 🐦 [BlueSky](https://bsky.app/profile/hatchman76.bsky.social)
- 📝 [Medium Blog](https://medium.com/@Hatchman76)
- 🌐 [opsguidance.hatchman76.com](https://opsguidance.hatchman76.com)

---

⭐ **If this presentation was helpful, please consider starring the repository!**