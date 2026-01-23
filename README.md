# Frontend Mentor - Intro section with dropdown navigation solution

This is a solution to the [Intro section with dropdown navigation challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-section-with-dropdown-navigation-ryaPetHE5). This project showcases a responsive landing page with complex dropdown navigation, built with modern web technologies.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Installation and Usage](#installation-and-usage)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Architecture](#architecture)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- **View dropdown menus**: Interact with navigation links to reveal dropdowns on both desktop and mobile.
- **Responsive Navigation**: Experience an optimal layout that adapts to device screen size, switching between a mobile drawer and a desktop horizontal menu.
- **Interactive Elements**: See distinct hover states for all interactive elements on the page.
- **Overlay Effects**: Observe a dimmed background overlay when the mobile menu is active.

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [GitHub Repository](https://github.com/bhzeuscagd/intro-section-with-dropdown-navigation-main)
- Live Site URL: [Vercel Deployment](https://intro-section-with-dropdown-navigation-main-3n17a9ly6.vercel.app)

## Installation and Usage

### Prerequisites
- [Node.js](https://nodejs.org/) (Latest LTS recommended)
- [pnpm](https://pnpm.io/) or npm

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/bhzeuscagd/intro-section-with-dropdown-navigation-main.git
   ```
2. Navigate to the project directory:
   ```bash
   cd intro-section-with-dropdown-navigation-main
   ```
3. Install dependencies:
   ```bash
   pnpm install
   ```

### Usage
Start the development server:
```bash
pnpm run dev
```
Open [http://localhost:4321](http://localhost:4321) in your browser to see the result.

## My process

### Built with

- [Astro](https://astro.build/) - Web framework for content-driven websites.
- [Tailwind CSS v4](https://tailwindcss.com/) - Utility-first CSS framework.
- [Fontsource](https://fontsource.org/) - Self-hosted Open Source fonts (Epilogue).
- Semantic HTML5 markup
- CSS Grid & Flexbox
- Mobile-first workflow

### Architecture

#### Component Map
The application is structured into modular Astro components to separate concerns and enhance maintainability:

- **`Layout`**: The main wrapper providing the HTML structure, metadata, and global font styles.
- **`Header`**: Contains the logo, navigation logic, and the mobile menu toggle.
  - **`Menu`**: Handles the recursive rendering of dropdown items and responsive behavior.
- **`HeroSection`**: The primary visual area of the landing page.
  - **`HeroContent`**: Displays the headline, description, and "Learn more" CTA.
  - **`HeroImage`**: Manages the responsive image switching (mobile vs. desktop assets).
- **`Clients`**: A logo strip showcasing client brands.
- **`UI Components`**: Reusable low-level components like `Button` and `Icons`.

#### Data Flow & Styling
- **Static Generation**: The site is statically generated for optimal performance and SEO.
- **Responsive Design**: Tailwind CSS utility classes are used to handle breakpoints, ensuring the layout shifts smoothly from mobile stacked views to desktop grid layouts.
- **State Management**: Minimal client-side JavaScript is used solely for toggling the mobile navigation drawer and dropdown visibility.

## Author
- Portfolio - [Cagd](https://portfolio-cagd.vercel.app/)
- Frontend Mentor - [@bhzeuscagd](https://www.frontendmentor.io/profile/bhzeuscagd)
- GitHub - [bhzeuscagd](https://github.com/bhzeuscagd)

## Acknowledgments
- [Frontend Mentor](https://www.frontendmentor.io) for the professional design resources and challenge.
- [Astro Docs](https://docs.astro.build) for the excellent documentation on component composition.
