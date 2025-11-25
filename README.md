# Moood 🌙✨

An interactive mood quiz web app where users swipe through affirmations to discover their mood of the day. Built with Next.js, React, and Framer Motion.

## 🎯 Overview

Moood is a swipe-based mood discovery quiz that presents 10 fun affirmations. Users swipe right for "yes" and left for "no" based on how each statement resonates with them. At the end, the app reveals their dominant mood from four unique personality types:

- **✨ Cosmic Chill** - Calm, grounded, effortlessly unbothered
- **🔥 Main Character Energy** - Confident, dramatic, self-assured
- **🌪 Chaotic Good** - Impulsive, creative, spontaneous
- **🌙 Soft Existential** - Reflective, dreamy, beautifully overthinking

## ✨ Features

- **Interactive Swipe Cards** - Smooth card-based interface with swipe gestures powered by Framer Motion
- **Real-time Feedback** - Visual feedback on swipe direction with animated text
- **Mood Calculation** - Intelligent algorithm to determine dominant mood based on affirmation responses
- **Results Sharing** - Share your mood result on Twitter, LinkedIn, Facebook, or via native share
- **Responsive Design** - Fully responsive UI that works on desktop and mobile devices
- **Elegant Animations** - Polished transitions and animations throughout the experience

## 🚀 Getting Started

### Prerequisites

- Node.js 20+ installed on your machine
- npm, yarn, pnpm, or bun package manager

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd moood
```

2. Install dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

3. Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

## 🛠 Tech Stack

- **Framework**: [Next.js 15.5.4](https://nextjs.org/) with React 19
- **Language**: TypeScript
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)
- **Build Tool**: Turbopack (Next.js built-in)
- **Linting**: ESLint with Prettier
- **Font Optimization**: Next.js Font system

## 📁 Project Structure

```
moood/
├── src/
│   ├── app/
│   │   ├── globals.css          # Global styles and design tokens
│   │   ├── layout.tsx           # Root layout component
│   │   ├── manifest.json        # PWA manifest
│   │   └── page.tsx             # Main page component
│   ├── components/
│   │   ├── card.tsx             # Swipeable card component
│   │   ├── results.tsx          # Results display and sharing
│   │   ├── start.tsx            # Welcome/start screen
│   │   ├── swiper.tsx           # Main swiper logic and state
│   │   └── index.ts             # Component exports
│   └── lib/
│       └── data.json            # Affirmations and mood definitions
├── public/
│   └── fonts/                   # Custom fonts
├── eslint.config.mjs
├── next.config.ts
├── postcss.config.mjs
├── tailwind.config.ts
└── tsconfig.json
```

## 🎨 Customization

### Adding New Affirmations

Edit `src/lib/data.json` to add or modify affirmations:

```json
{
    "id": 11,
    "text": "Your custom affirmation here",
    "moods": ["cosmicChill", "mainCharacter"]
}
```

### Modifying Mood Types

Update the `moods` object in `src/lib/data.json` to customize mood descriptions, names, and emojis.

### Styling

The design system is defined in `src/app/globals.css` using CSS custom properties. Modify the `:root` variables to change colors, typography, and spacing.

## 📜 Available Scripts

- `npm run dev` - Start development server with Turbopack
- `npm run build` - Build for production with Turbopack
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## 🚢 Deployment

The easiest way to deploy is using [Vercel](https://vercel.com):

1. Push your code to a Git repository
2. Import your project to Vercel
3. Vercel will automatically detect Next.js and configure the build
4. Deploy!

For other platforms, build the project with `npm run build` and deploy the `.next` folder.

## 🎯 Future Enhancements

- [ ] More affirmations and mood types
- [ ] Keyboard navigation support

## 📄 License

This project is private and not currently licensed for public use.
