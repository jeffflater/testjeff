# TestJeff

**Smart Test Automation Made Simple** - A technical authority hub for software testing education, courses, and open-source projects.

## 🚀 About

TestJeff is a brand and education platform created by Jeff Flater, focused on helping software testers, QA engineers, and automation professionals level up their skills with modern tools, smart workflows, and AI-powered testing.

**Live Site:** [testjeff.com](https://testjeff.com)

## 🛠️ Tech Stack

- **Static Site Generator:** Jekyll
- **Hosting:** GitHub Pages
- **Theme:** Custom dark theme with technical aesthetics
- **Styling:** SCSS with modern CSS features
- **Typography:** Inter (body) + JetBrains Mono (code/technical)

## 📦 Local Development Setup

You have **two options** for running the site locally:

### Option 1: Using Docker (Recommended - Easiest)

**Prerequisites:** [Docker Desktop](https://www.docker.com/products/docker-desktop)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/jeffflater/testjeff.git
   cd testjeff
   ```

2. **Start the development server:**
   ```bash
   docker-compose up
   ```

3. **Open your browser:**
   ```
   http://localhost:4000
   ```

4. **Stop the server:**
   ```bash
   # Press Ctrl+C in the terminal, then:
   docker-compose down
   ```

✨ **Benefits:**
- No Ruby installation needed
- No dependency issues
- Works the same on all operating systems
- Automatic live reload when you edit files

---

### Option 2: Using Ruby (Native)

**Prerequisites:**
- **Ruby** (2.7 or higher) - [Install Ruby](https://www.ruby-lang.org/en/documentation/installation/)
- **Bundler** - Install with: `gem install bundler`

**Note:** If you're on macOS with Apple Silicon and Ruby 3.3+, you may encounter build errors with `eventmachine`. Use the Docker method instead.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/jeffflater/testjeff.git
   cd testjeff
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   ```

3. **Run the local development server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **Open your browser:**
   ```
   http://localhost:4000
   ```

### Development Commands (Ruby)

- **Build site:** `bundle exec jekyll build`
- **Serve with drafts:** `bundle exec jekyll serve --drafts`
- **Clean build files:** `bundle exec jekyll clean`

## 📁 Project Structure

```
testjeff/
├── _config.yml           # Jekyll configuration
├── _includes/            # Reusable HTML components
│   ├── head-custom.html
│   └── sidebar.html
├── _layouts/             # Page templates
│   └── sidebar.html
├── _posts/               # Blog posts (Markdown)
├── assets/
│   ├── css/
│   │   └── style.scss    # All custom styles
│   └── img/              # Images and logos
├── about.md              # About page
├── blog.md               # Blog index
├── courses.md            # Courses landing page
├── github.md             # GitHub projects
├── index.md              # Homepage
└── CNAME                 # Custom domain config
```

## 🎨 Design Philosophy

The site uses a **dark, technical aesthetic** designed to:
- Position TestJeff as a testing authority
- Appeal to software testers and QA engineers
- Showcase technical credibility through design
- Provide a creative, modern user experience

### Color Palette

- **Primary:** `#00D9FF` (Cyan - test pass indicator)
- **Secondary:** `#A78BFA` (Purple - creative accent)
- **Background:** `#0A0E27` (Deep space blue-black)
- **Success:** `#10B981` (Green)
- **Warning:** `#F59E0B` (Orange)
- **Error:** `#EF4444` (Red)

## ✍️ Creating Content

### New Blog Post

Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

```markdown
---
layout: sidebar
title: Your Post Title
date: 2025-01-15
---

Your content here...
```

### New Page

Create a new `.md` file in the root directory:

```markdown
---
layout: sidebar
title: Page Title
---

Your content here...
```

## 🚀 Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch.

To deploy changes:
```bash
git add .
git commit -m "Your commit message"
git push origin main
```

GitHub Pages will rebuild the site automatically (takes 1-2 minutes).

## 📝 License

© 2025 Jeff Flater / TestJeff. All rights reserved.

## 🤝 Contact

- **Website:** [testjeff.com](https://testjeff.com)
- **GitHub:** [@jeffflater](https://github.com/jeffflater)
- **Udemy:** [TestJeff Courses](https://www.udemy.com/user/jeff-flater/)

---

Built with Jekyll • Hosted on GitHub Pages • Designed for Testing Professionals
