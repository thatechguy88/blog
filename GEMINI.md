# Gemini Instructions: Astro Blog

This project is a blog built with [Astro](https://astro.build/) using MDX for content and Content Collections for structured data.

## Tech Stack
- **Framework:** Astro 5
- **Content:** MDX (`@astrojs/mdx`)
- **Metadata:** Sitemap (`@astrojs/sitemap`), RSS (`@astrojs/rss`)
- **Type Safety:** TypeScript + Zod (for content schemas)
- **Styling:** Standard CSS (found in `src/styles/`)

## Core Project Structure
- `src/content/blog/`: Markdown and MDX blog posts.
- `src/content.config.ts`: Defines the schema for the blog collection.
- `src/pages/blog/`: Contains the blog index and dynamic post route (`[...slug].astro`).
- `src/layouts/`: Reusable page layouts, primarily `BlogPost.astro`.
- `src/components/`: Reusable Astro components for the UI.

## Development Guidelines
- **Content:** When adding a new blog post, ensure it follows the schema defined in `src/content.config.ts` (title, description, pubDate, heroImage).
- **Styling:** Use the global styles in `src/styles/global.css` or component-specific styles.
- **Components:** Prefer Astro components for static UI and only use framework components (React, etc.) if interactivity is required (none currently used).

## Common Commands
- `npm run dev`: Start the development server.
- `npm run build`: Build the project for production.
- `npm run preview`: Preview the production build locally.
- `npx astro check`: Run type checking on the Astro project.
