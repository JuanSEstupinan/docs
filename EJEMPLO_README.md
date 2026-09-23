# NASA Astronomy Pictures Web Application

Web application developed for the National Aeronautics and Space Administration (NASA) to display daily and historical astronomical pictures using the NASA APOD API.

---

## 1. Project Information
- **Course:** Web Applications (1ASI0730)
- **Evaluation:** Practical Assessment 1 (PC1) - Term 2025-2
- **Project Name:** `pc17432u[your-code]`
- **Framework & Tooling:** Vue 3 (Composition API), Vite, WebStorm

---

## 2. Description
This application provides scientific outreach and exploration by retrieving and presenting Astronomy Picture of the Day (APOD) entries from NASA's public REST API. The system displays high-resolution space images and videos, metadata, and detailed scientific explanations, allowing international users to switch between English and Spanish seamlessly.

The codebase adheres to a Domain-Driven Design (DDD) layered architecture, separating concerns into `shared` and `apod` bounded contexts, with clean separation between presentation, application, domain, and infrastructure layers. It implements design patterns such as Request/Response, Resource, and Assembler.

---

## 3. Features
- **Top Toolbar:**
  - Dynamic NASA logo integration retrieved via Clearbit Logo API (`https://logo.clearbit.com/nasa.gov`).
  - Institution title and accessible layout.
  - Interactive language selector (`EN | ES`) powered by `vue-i18n` (English set by default).
- **Astronomy Pictures Grid:**
  - Responsive cards displaying NASA APOD data: title, date, explanation, and media content.
  - Support for both image and video media types with a reliable generic placeholder fallback.
  - "See on NASA" external button converting picture titles to `kebab-case` and redirecting users to the official NASA APOD page in a new browser tab (`https://apod.nasa.gov/apod/<kebab-case-title>`).
- **Footer Section:**
  - First line: `"Copyright ©2025 The NASA, inc All rights reserved."`
  - Second line: Developer attribution `"Developed by [Student Code] - [Student Full Name]"`.
- **Accessibility & UX:**
  - Accessible Rich Internet Applications (ARIA) attributes across interactive elements and views.
  - Responsive layout utilizing PrimeFlex and Material theme styles.

---

## 4. Dependencies
The application relies on the following core production dependencies:

- **[Vue 3](https://vuejs.org/):** Progressive JavaScript frontend framework using the Composition API.
- **[PrimeVue](https://primevue.org/):** UI component suite styled with the Material theme (registered with `pv-` prefix).
- **[PrimeFlex](https://primeflex.org/):** Utility-based CSS library for grid and flexbox responsive layouts.
- **[PrimeIcons](https://primevue.org/icons):** Icon library for PrimeVue components.
- **[Axios](https://axios-http.com/):** Promise-based HTTP client for consuming the NASA APOD API.
- **[Vue-i18n](https://vue-i18n.intlify.dev/):** Internationalization framework for multi-language support (EN/ES).

### Dev Dependencies
- **[Vite](https://vitejs.dev/):** Next-generation frontend tooling and local dev server.

---

## 5. Getting Started

### Prerequisites
- Node.js (version 18.x or higher recommended)
- npm (version 9.x or higher)

### Installation
Clone or extract the project repository, navigate to the root directory, and install dependencies:
```bash
npm install
```

### Development Server
Run the local development server:
```bash
npm run dev
```

### Production Build
Compile and bundle the project for production deployment:
```bash
npm run build
```

---

## 6. Author Information
- **Student Code:** u[your-code-here]
- **Full Name:** [Your First and Last Name]
- **NRC:** 7432
- **Profesor:** Sánchez Ponce, Alex Humberto
