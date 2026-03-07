# Gemini Instructions: Astro Blog

This project is a Frutiger Aero-themed blog built with [Astro](https://astro.build/) using MDX for content and Content Collections for structured data.

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
- `src/assets/`: Visual assets like background images and icons.

## Development Guidelines
- **Aesthetic:** Maintain the Frutiger Aero look (glossy textures, nature-inspired backgrounds, vibrant colors). Background images are managed in `src/styles/global.css`.
- **Content:** When adding a new blog post, ensure it follows the schema defined in `src/content.config.ts` (title, description, pubDate, heroImage).
- **Styling:** Use the global styles in `src/styles/global.css` or component-specific styles.
- **Components:** Prefer Astro components for static UI.

## Git Workflow
To push changes to the repository:
1. `git status`: Check modified/new files.
2. `git add <file>`: Stage changes for commit.
3. `git commit -m "feat/fix/style: message"`: Create a local commit.
4. `git push origin main`: Upload changes to the remote repository.

## Common Commands
- `npm run dev`: Start the development server.
- `npm run build`: Build the project for production.
- `npm run preview`: Preview the production build locally.
- `npx astro check`: Run type checking on the Astro project.
