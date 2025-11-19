# Ali Fouladgar - Personal Portfolio

A modern, minimalist, and high-performance personal portfolio website built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com). Designed to showcase professional experience, projects, and technical expertise with a clean, dark-mode-first aesthetic.

## 🚀 Tech Stack

- **Framework:** [Astro](https://astro.build) - For blazing fast performance and component-based architecture.
- **Styling:** [Tailwind CSS](https://tailwindcss.com) - Utility-first CSS framework for rapid UI development.
- **Language:** [TypeScript](https://www.typescriptlang.org/) - For type-safe code.
- **Icons:** Custom SVG icons.
- **Font:** [Inter](https://rsms.me/inter/) - Variable font for optimal typography.

## ✨ Features

- **Minimalist Design:** Clean, high-contrast aesthetic inspired by modern developer portfolios.
- **Dark/Light Mode:** Fully supported theme toggling with system preference detection.
- **Responsive Layout:** Optimized for all device sizes, from mobile to desktop.
- **Smooth Animations:** Scroll-triggered fade-in and slide-up effects for a polished user experience.
- **Dynamic Background:** Subtle grid patterns that adapt to the theme.
- **SEO Optimized:** Proper meta tags, semantic HTML, and fast load times.

## 🛠️ Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm, pnpm, or yarn

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/amfooladgar/portfolio.git
   cd portfolio
   ```

2. **Install dependencies:**

   ```bash
   npm install
   # or
   pnpm install
   ```

3. **Start the development server:**

   ```bash
   npm run dev
   # or
   pnpm dev
   ```

   The site will be available at `http://localhost:4321`.

### Building for Production

To create a production build:

```bash
npm run build
# or
pnpm build
```

## 📂 Project Structure

```text
src/
├── components/    # Reusable UI components (Header, Footer, Sections)
├── layouts/       # Page layouts (Layout.astro)
├── pages/         # Route definitions (index.astro)
├── styles/        # Global styles, patterns, and animations
└── env.d.ts       # TypeScript environment definitions
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE.md).
