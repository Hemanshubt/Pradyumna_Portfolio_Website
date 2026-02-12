# Developer Portfolio

A modern, responsive Developer Portfolio website built with Next.js 14, Tailwind CSS, and various integrations for contact and analytics.

## Features

- ⚡ **Next.js 14**: Utilizing the App Router for efficient and modern routing.
- 🎨 **Tailwind CSS**: Rapid and responsive UI development.
- 📝 **Blog Integration**: Fetch and display blog posts (e.g., from Dev.to).
- 📧 **Contact Form**: Integrated with Nodemailer and Telegram for instant notifications.
- 🤖 **ReCaptcha**: Secured with Google ReCaptcha.
- 📊 **Analytics**: Integrated with Google Tag Manager.
- 🐳 **Dockerized**: specific Dockerfiles for development and production.
- 📱 **Responsive Design**: Mobile-first approach.

## Tech Stack

- **Framework**: [Next.js](https://nextjs.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) & [Sass](https://sass-lang.com/)
- **Animations**: [Lottie React](https://lottiefiles.com/blog/working-with-lottie/getting-started-with-lottie-react) & [React Fast Marquee](https://www.react-fast-marquee.com/)
- **HTTP Client**: [Axios](https://axios-http.com/)
- **Notifications**: [React Toastify](https://fkhadra.github.io/react-toastify/)

## Project Structure

```
├── app/                # Next.js App Router directories
│   ├── api/            # API routes
│   ├── assets/         # Static assets and images
│   ├── blog/           # Blog page components
│   ├── components/     # Reusable React components
│   ├── css/            # Global styles
│   ├── layout.js       # Root layout
│   └── page.js         # Home page
├── public/             # Static files served from root
├── utils/              # Utility functions and data
│   └── data/           # Static data (skills, projects, etc.)
├── .env.local          # Environment variables
├── next.config.js      # Next.js configuration
├── package.json        # Project dependencies and scripts
└── tailwind.config.js  # Tailwind CSS configuration
```

## Getting Started

### Prerequisites

- Node.js (v18 or later recommended)
- npm or yarn
- Docker (optional, for containerized run)

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd Pradyumna_Portfolio_Website
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

3.  **Set up Environment Variables:**

    Rename the `.env.example` file to `.env.local` and update the values with your own keys:

    ```bash
    cp .env.example .env.local
    ```

    **Required Variables:**

    - **Google Services:**
        - `NEXT_PUBLIC_GTM`: Your [Google Tag Manager](https://tagmanager.google.com/) Container ID.
        - `NEXT_PUBLIC_RECAPTCHA_SITE_KEY`: Site key from [Google reCAPTCHA](https://www.google.com/recaptcha/admin).
        - `NEXT_PUBLIC_RECAPTCHA_SECRET_KEY`: Secret key from [Google reCAPTCHA](https://www.google.com/recaptcha/admin).

    - **Email (Nodemailer):**
        - `EMAIL_ADDRESS`: The Gmail address used to send emails.
        - `GMAIL_PASSKEY`: An [App Password](https://myaccount.google.com/apppasswords) for the Gmail account (NOT your login password).

    - **Telegram Notifications:**
        - `TELEGRAM_BOT_TOKEN`: Token from [@BotFather](https://t.me/botfather).
        - `TELEGRAM_CHAT_ID`: Your chat ID (can be found using `@userinfobot`).

    - **General:**
        - `NEXT_PUBLIC_BASE_URL`: The URL of your deployed site (e.g., `https://your-portfolio.com`).


### Running Locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Building for Production

```bash
npm run build
npm start
```

## Docker

### Running with Docker Compose

This project includes a `docker-compose.yml` for easy setup.

```bash
docker-compose up -d --build
```

### Building Docker Image Manually

**Development:**

```bash
docker build -t portfolio-dev -f Dockerfile.dev .
docker run -p 3000:3000 portfolio-dev
```

**Production:**

```bash
docker build -t portfolio-prod -f Dockerfile.prod .
docker run -p 3000:3000 portfolio-prod
```

## Deployment

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Alternatively, since `netlify.toml` is present, you can easily deploy to [Netlify](https://www.netlify.com/).

## License

This project is licensed under the MIT License.
