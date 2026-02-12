# 🚀 Developer Portfolio - Pradyumna Marathe

<div align="center">

![Next.js](https://img.shields.io/badge/Next.js-14.1.0-black?style=for-the-badge&logo=next.js)
![React](https://img.shields.io/badge/React-18.2.0-61DAFB?style=for-the-badge&logo=react)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4.1-38B2AC?style=for-the-badge&logo=tailwind-css)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker)

A modern, fully responsive Machine Learning Engineer portfolio showcasing projects, skills, experience, and education with integrated contact functionality and smooth animations.

[Live Demo](https://your-portfolio.com) • [Report Bug](https://github.com/Hemanshubt/Pradyumna_Portfolio_Website/issues) • [Request Feature](https://github.com/Hemanshubt/Pradyumna_Portfolio_Website/issues)

</div>

---

## ✨ Features

### 🎯 Core Features
- ⚡ **Next.js 14 App Router**: Server-side rendering with the latest Next.js features
- 🎨 **Modern UI/UX**: Beautiful gradient designs with Tailwind CSS and custom SCSS
- 📱 **Fully Responsive**: Mobile-first design that works on all devices
- 🌙 **Smooth Animations**: Lottie animations and React Fast Marquee for engaging visuals
- 🚀 **Performance Optimized**: Image optimization with Next.js Image component
- 🔒 **Production Ready**: Console removal in production builds

### 📬 Contact & Communication
- 📧 **Dual Notification System**: Email (Nodemailer) + Telegram Bot integration
- 🤖 **Google reCAPTCHA**: Spam protection for contact forms
- 💌 **HTML Email Templates**: Professional styled email notifications
- ⚡ **Real-time Notifications**: Instant Telegram alerts for new messages

### 📊 Content Sections
- 👤 **Hero Section**: Animated introduction with social links
- 💼 **Experience Timeline**: Professional work history
- 🎓 **Education**: Academic background with visual cards
- 🛠️ **Skills Showcase**: Animated skill icons with marquee effect
- 📁 **Projects Gallery**: Portfolio projects with detailed cards
- 📝 **Blog Integration**: Fetch and display blog posts from Dev.to
- 📞 **Contact Form**: Integrated contact with validation

### 🐳 DevOps & Deployment
- 🐳 **Docker Support**: Separate Dockerfiles for dev and production
- 📦 **Docker Compose**: One-command setup
- 🌐 **Multi-Platform Deploy**: Vercel, Netlify, and standalone deployment
- 🔧 **Environment Config**: Secure environment variable management

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose | Version |
|------------|---------|---------|
| [Next.js](https://nextjs.org/) | React Framework | 14.1.0 |
| [React](https://react.dev/) | UI Library | 18.2.0 |
| [Tailwind CSS](https://tailwindcss.com/) | Utility-first CSS | 3.4.1 |
| [Sass](https://sass-lang.com/) | CSS Preprocessor | 1.69.5 |

### Libraries & Tools
| Library | Purpose |
|---------|---------|
| [Lottie React](https://www.npmjs.com/package/lottie-react) | JSON-based animations |
| [React Fast Marquee](https://www.react-fast-marquee.com/) | Smooth scrolling marquee |
| [React Icons](https://react-icons.github.io/react-icons/) | Icon library |
| [React Toastify](https://fkhadra.github.io/react-toastify/) | Toast notifications |
| [Axios](https://axios-http.com/) | HTTP client |
| [Sharp](https://sharp.pixelplumbing.com/) | Image optimization |

### Backend & APIs
| Service | Purpose |
|---------|---------|
| [Nodemailer](https://nodemailer.com/) | Email sending |
| [Telegram Bot API](https://core.telegram.org/bots/api) | Instant notifications |
| [Google reCAPTCHA](https://www.google.com/recaptcha/) | Form security |
| [EmailJS](https://www.emailjs.com/) | Alternative email service |

### DevOps
- **Docker**: Containerization
- **Docker Compose**: Multi-container orchestration
- **Netlify**: Deployment platform
- **Vercel**: Deployment platform

---

## 📁 Project Structure

```
Pradyumna_Portfolio_Website/
├── app/
│   ├── api/                          # API Routes
│   │   ├── contact/                  # Contact form handler
│   │   │   └── route.js              # POST endpoint for messages
│   │   ├── data/                     # Data fetching endpoints
│   │   │   └── route.js
│   │   └── google/                   # Google services integration
│   │       └── route.js
│   ├── assets/
│   │   ├── lottie/                   # Lottie animation JSON files
│   │   │   ├── build.json
│   │   │   ├── code.json
│   │   │   ├── coding.json
│   │   │   ├── contact.json
│   │   │   ├── development.json
│   │   │   ├── education.json
│   │   │   └── ...
│   │   └── svg/                      # SVG assets
│   │       ├── education/            # Education section icons
│   │       ├── experience/           # Experience section icons
│   │       ├── projects/             # Project thumbnails
│   │       └── skills/               # 80+ skill icons
│   ├── blog/                         # Blog page
│   │   └── page.js
│   ├── components/
│   │   ├── footer.jsx                # Footer component
│   │   ├── navbar.jsx                # Navigation bar
│   │   ├── helper/                   # Utility components
│   │   │   ├── animation-lottie.jsx  # Lottie wrapper
│   │   │   ├── glow-card.jsx         # Glowing card effect
│   │   │   └── scroll-to-top.jsx     # Scroll button
│   │   └── homepage/                 # Homepage sections
│   │       ├── about/                # About section
│   │       ├── blog/                 # Blog cards
│   │       ├── contact/              # Contact form
│   │       ├── education/            # Education timeline
│   │       ├── experience/           # Experience timeline
│   │       ├── hero-section/         # Hero/landing section
│   │       ├── projects/             # Projects gallery
│   │       └── skills/               # Skills showcase
│   ├── css/
│   │   ├── card.scss                 # Card styles
│   │   └── globals.scss              # Global styles
│   ├── layout.js                     # Root layout with metadata
│   ├── page.js                       # Homepage
│   ├── not-found.jsx                 # 404 page
│   └── favicon.ico
├── public/                           # Static assets
│   ├── image/                        # Project images
│   ├── png/                          # PNG assets
│   ├── profile.jpeg                  # Profile photo
│   ├── hero.svg                      # Hero background
│   └── ...
├── utils/
│   ├── data/                         # Data files
│   │   ├── personal-data.js          # Personal information
│   │   ├── educations.js             # Education data
│   │   ├── experience.js             # Work experience
│   │   ├── projects-data.js          # Projects list
│   │   ├── skills.js                 # Skills array
│   │   └── contactsData.js           # Contact info
│   ├── check-email.js                # Email validation
│   ├── skill-image.js                # Skill icon mapper
│   └── time-converter.js             # Date utilities
├── .env.example                      # Environment variables template
├── .env.local                        # Local environment (gitignored)
├── docker-compose.yml                # Docker Compose config
├── Dockerfile.dev                    # Development Docker image
├── Dockerfile.prod                   # Production Docker image
├── next.config.js                    # Next.js configuration
├── tailwind.config.js                # Tailwind CSS config
├── postcss.config.js                 # PostCSS config
├── jsconfig.json                     # JavaScript config
├── netlify.toml                      # Netlify deployment config
├── package.json                      # Dependencies
└── README.md                         # This file
```

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js**: v18.0.0 or later ([Download](https://nodejs.org/))
- **npm**: v9.0.0 or later (comes with Node.js)
- **Git**: For cloning the repository ([Download](https://git-scm.com/))
- **Docker** (Optional): For containerized deployment ([Download](https://www.docker.com/))

### 📥 Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/Hemanshubt/Pradyumna_Portfolio_Website.git
cd Pradyumna_Portfolio_Website
```

#### 2. Install Dependencies

```bash
npm install
```

#### 3. Configure Environment Variables

Create a `.env.local` file from the example template:

```bash
# Windows (CMD)
copy .env.example .env.local

# Windows (PowerShell)
Copy-Item .env.example .env.local

# Linux/Mac
cp .env.example .env.local
```

Edit `.env.local` with your credentials:

```env
# Contact Form (Nodemailer)
EMAIL_ADDRESS=your_email@gmail.com
GMAIL_PASSKEY=your_gmail_app_password

# Telegram Notifications
TELEGRAM_BOT_TOKEN=your_bot_token
TELEGRAM_CHAT_ID=your_chat_id

# Base URL
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

---

## 🔑 Environment Variables Setup Guide

### 📧 Email Configuration (Nodemailer)

#### `EMAIL_ADDRESS`
Your Gmail address that will receive contact form submissions.

**Example**: `marathepradyumna744@gmail.com`

#### `GMAIL_PASSKEY`
A 16-character App Password (NOT your regular Gmail password).

**How to get it**:
1. Go to [Google Account Security](https://myaccount.google.com/security)
2. Enable **2-Step Verification** (if not already enabled)
3. Navigate to **2-Step Verification** → **App passwords** (at the bottom)
4. Select **Mail** and your device
5. Click **Generate**
6. Copy the 16-character password (format: `xxxx xxxx xxxx xxxx`)

**Example**: `abcd efgh ijkl mnop`

---

### 📱 Telegram Bot Configuration

#### `TELEGRAM_BOT_TOKEN`
Your Telegram bot's API token for sending notifications.

**How to get it**:
1. Open Telegram and search for [@BotFather](https://t.me/botfather)
2. Send the command `/newbot`
3. Follow the prompts:
   - Choose a name for your bot (e.g., "Portfolio Contact Bot")
   - Choose a username (must end in 'bot', e.g., "pradyumna_portfolio_bot")
4. Copy the **HTTP API token** provided

**Example**: `1234567890:ABCdefGHIjklMNOpqrsTUVwxyz123456789`

#### `TELEGRAM_CHAT_ID`
Your personal Telegram chat ID where notifications will be sent.

**How to get it**:
1. Open Telegram and search for [@userinfobot](https://t.me/userinfobot)
2. Start the bot by clicking **Start**
3. The bot will reply with your user information
4. Copy the **Id** number

**Alternative method**:
1. Send a message to your bot
2. Visit: `https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates`
3. Look for `"chat":{"id":123456789}` in the response
4. Copy the ID number

**Example**: `123456789`

---

### 🌐 Application URL

#### `NEXT_PUBLIC_APP_URL`
The base URL of your application.

**Development**: `http://localhost:3000`  
**Production**: `https://your-domain.com`

---

## 💻 Development

### Run Development Server

```bash
npm run dev
```

The application will be available at [http://localhost:3000](http://localhost:3000)

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Build optimized production bundle |
| `npm start` | Start production server |
| `npm run lint` | Run ESLint for code quality checks |

### Build for Production

```bash
# Create optimized production build
npm run build

# Start production server
npm start
```

The production build includes:
- ✅ Optimized bundle size
- ✅ Image optimization
- ✅ Console logs removed
- ✅ Minified CSS and JavaScript

---

## 🐳 Docker Deployment

This project includes Docker support for both development and production environments.

### Quick Start with Docker Compose

The easiest way to run the application with Docker:

```bash
# Build and start the container
docker-compose up -d --build

# View logs
docker-compose logs -f

# Stop the container
docker-compose down
```

The application will be available at [http://localhost:3000](http://localhost:3000)

### Manual Docker Build

#### Development Environment

```bash
# Build development image
docker build -t portfolio-dev -f Dockerfile.dev .

# Run development container
docker run -p 3000:3000 --env-file .env.local portfolio-dev
```

#### Production Environment

```bash
# Build production image
docker build -t portfolio-prod -f Dockerfile.prod .

# Run production container
docker run -p 3000:3000 --env-file .env.local portfolio-prod
```

### Docker Configuration

**Dockerfile.dev**: Development environment with hot reload  
**Dockerfile.prod**: Optimized production build with standalone output  
**docker-compose.yml**: Orchestration configuration

---

## 🌐 Deployment Options

### Deploy to Vercel (Recommended)

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Hemanshubt/Pradyumna_Portfolio_Website)

1. Click the button above or go to [Vercel](https://vercel.com/new)
2. Import your GitHub repository
3. Configure environment variables in Vercel dashboard
4. Deploy!

**Advantages**:
- ✅ Zero configuration
- ✅ Automatic HTTPS
- ✅ Global CDN
- ✅ Automatic deployments on git push

### Deploy to Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Hemanshubt/Pradyumna_Portfolio_Website)

1. Click the button above or drag your project folder to [Netlify](https://app.netlify.com/)
2. Configure build settings (already set in `netlify.toml`)
3. Add environment variables in Netlify dashboard
4. Deploy!

**Build Settings** (auto-configured via `netlify.toml`):
- Build command: `npm run build`
- Publish directory: `.next`

### Self-Hosted Deployment

#### Using PM2 (Process Manager)

```bash
# Install PM2 globally
npm install -g pm2

# Build the application
npm run build

# Start with PM2
pm2 start npm --name "portfolio" -- start

# Save PM2 configuration
pm2 save

# Setup PM2 to start on system boot
pm2 startup
```

#### Using Docker in Production

```bash
# Build production image
docker build -t portfolio-prod -f Dockerfile.prod .

# Run with restart policy
docker run -d \
  --name portfolio \
  --restart unless-stopped \
  -p 3000:3000 \
  --env-file .env.local \
  portfolio-prod
```

---

## 🎨 Customization Guide

### Update Personal Information

Edit `utils/data/personal-data.js`:

```javascript
export const personalData = {
  name: "YOUR NAME",
  profile: '/profile.jpeg',
  designation: "Your Job Title",
  description: "Your bio...",
  email: 'your.email@example.com',
  phone: '+1234567890',
  address: 'Your Location',
  github: 'https://github.com/yourusername',
  linkedIn: 'https://www.linkedin.com/in/yourusername/',
  twitter: 'https://twitter.com/yourusername',
  resume: "https://your-resume-link.com"
}
```

### Add/Update Skills

Edit `utils/data/skills.js`:

```javascript
export const skills = [
  { name: 'Python', icon: 'python.svg' },
  { name: 'JavaScript', icon: 'javascript.svg' },
  // Add more skills...
]
```

Add corresponding SVG icons to `app/assets/svg/skills/`

### Add Projects

Edit `utils/data/projects-data.js`:

```javascript
export const projectsData = [
  {
    id: 1,
    name: 'Project Name',
    description: "Project description...",
    tools: ['React', 'Node.js', 'MongoDB'],
    role: 'Full Stack Developer',
    code: 'https://github.com/username/repo',
    demo: 'https://demo-link.com',
    image: '/image/project.jpg',
  },
  // Add more projects...
]
```

### Update Experience

Edit `utils/data/experience.js`:

```javascript
export const experiences = [
  {
    id: 1,
    title: 'Job Title',
    company: "Company Name",
    duration: "(Jan 2023 - Present)"
  },
  // Add more experiences...
]
```

### Update Education

Edit `utils/data/educations.js`:

```javascript
export const educations = [
  {
    id: 1,
    title: "Degree Name",
    duration: "2020 - 2024",
    institution: "University Name",
  },
  // Add more education entries...
]
```

### Change Color Scheme

Edit `tailwind.config.js` or modify gradient colors in components:

```javascript
// Common gradient classes used:
// from-pink-500 to-violet-600
// from-[#0d1224] to-[#0a0d37]
// text-[#16f2b3]
```

### Add Custom Animations

Place Lottie JSON files in `app/assets/lottie/` and use the `AnimationLottie` component:

```jsx
import AnimationLottie from '../helper/animation-lottie';
import myAnimation from '@/app/assets/lottie/my-animation.json';

<AnimationLottie animationPath={myAnimation} />
```

---

## 📂 Key Files Explained

| File | Purpose |
|------|---------|
| `app/layout.js` | Root layout with metadata, fonts, and global providers |
| `app/page.js` | Homepage that imports all section components |
| `app/api/contact/route.js` | API endpoint handling contact form submissions |
| `utils/data/personal-data.js` | Your personal information and social links |
| `utils/data/projects-data.js` | Portfolio projects data |
| `utils/data/skills.js` | Skills array for the skills section |
| `utils/data/experience.js` | Work experience timeline data |
| `utils/data/educations.js` | Education history data |
| `next.config.js` | Next.js configuration (images, output, optimization) |
| `tailwind.config.js` | Tailwind CSS customization |
| `docker-compose.yml` | Docker orchestration configuration |

---

## 🔧 Troubleshooting

### Common Issues

#### Port Already in Use

```bash
# Windows
netstat -ano | findstr :3000
taskkill /PID <PID> /F

# Linux/Mac
lsof -ti:3000 | xargs kill -9
```

#### Environment Variables Not Loading

- Ensure `.env.local` exists in the root directory
- Restart the development server after changing environment variables
- Check that variable names match exactly (case-sensitive)

#### Email Not Sending

- Verify Gmail App Password is correct (16 characters, no spaces)
- Ensure 2-Step Verification is enabled on your Google account
- Check that `EMAIL_ADDRESS` matches the account that generated the App Password

#### Telegram Notifications Not Working

- Verify bot token is correct
- Ensure you've started a conversation with your bot (send `/start`)
- Confirm chat ID is correct (use [@userinfobot](https://t.me/userinfobot))
- Check bot has permission to send messages

#### Build Errors

```bash
# Clear Next.js cache
rm -rf .next

# Clear node_modules and reinstall
rm -rf node_modules package-lock.json
npm install

# Clear npm cache
npm cache clean --force
```

#### Docker Issues

```bash
# Remove all containers and images
docker-compose down --rmi all --volumes

# Rebuild from scratch
docker-compose up --build --force-recreate
```

---

## 📊 Performance Optimization

This portfolio is optimized for performance:

- ✅ **Next.js Image Optimization**: Automatic image optimization and lazy loading
- ✅ **Code Splitting**: Automatic code splitting with Next.js App Router
- ✅ **Production Build**: Minified CSS/JS, console removal
- ✅ **Standalone Output**: Minimal production bundle
- ✅ **Package Optimization**: Experimental package import optimization
- ✅ **Remote Image Patterns**: Configured for Cloudinary and Dev.to images

### Lighthouse Scores Target

- Performance: 90+
- Accessibility: 95+
- Best Practices: 95+
- SEO: 100

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/AmazingFeature`
3. **Commit your changes**: `git commit -m 'Add some AmazingFeature'`
4. **Push to the branch**: `git push origin feature/AmazingFeature`
5. **Open a Pull Request**

### Contribution Guidelines

- Follow the existing code style
- Write clear commit messages
- Update documentation as needed
- Test your changes thoroughly
- Ensure all environment variables are documented

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Pradyumna Marathe**

- Portfolio: [your-portfolio.com](https://your-portfolio.com)
- GitHub: [@Pradyumna744](https://github.com/Pradyumna744)
- LinkedIn: [pradyumna744](https://www.linkedin.com/in/pradyumna744/)
- Twitter: [@PRADYUMNA_744](https://x.com/PRADYUMNA_744)
- Email: marathepradyumna744@gmail.com

---

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) - The React Framework
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Lottie Files](https://lottiefiles.com/) - Animation library
- [React Icons](https://react-icons.github.io/) - Icon library
- [Vercel](https://vercel.com/) - Deployment platform

---

## 📞 Support

If you have any questions or need help, feel free to:

- Open an [Issue](https://github.com/Hemanshubt/Pradyumna_Portfolio_Website/issues)
- Contact via [Email](mailto:marathepradyumna744@gmail.com)
- Connect on [LinkedIn](https://www.linkedin.com/in/pradyumna744/)

---

<div align="center">

### ⭐ Star this repository if you found it helpful!

Made with ❤️ by [Pradyumna Marathe](https://github.com/Pradyumna744)

</div>
