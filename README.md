# Astro Resume

## Features

- Astro v4
- TailwindCSS utility classes
- ESLint / Prettier pre-installed and pre-configured
- Accessible, semantic HTML markup
- Responsive & SEO-friendly
- Dark / Light mode, using Tailwind and CSS variables (referenced from shadcn)
- [Astro Assets Integration](https://docs.astro.build/en/guides/assets/) for optimised images
- MD & [MDX](https://docs.astro.build/en/guides/markdown-content/#mdx-only-features) posts
- Pagination
- [Automatic RSS feed](https://docs.astro.build/en/guides/rss)
- Auto-generated [sitemap](https://docs.astro.build/en/guides/integrations-guide/sitemap/)
- [Expressive Code](https://expressive-code.com/) source code and syntax highlighter

## Credits

- [astro-theme-cactus](https://github.com/chrismwilliams/astro-theme-cactus) for blog design
- [minirezume-framer](https://minirezume.framer.website/) for resume homepage design

## Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
├── public/
├── src/
    ├── assets/
│   ├── components/
│   ├── content/
│   ├── layouts/
|   ├── pages/
|   ├── styles/
|   ├── utils/
|   ├── site.config.ts
│   └── types.ts
├── .elintrc.cjs
├── .gitignore
├── .prettierignore
├── package.json
├── prettier.config.cjs
├── README.md
├── tailwind.config.js
└── tsconfig.json
```

## Editing guide

### Site info

To edit site info such as site title and description, edit the `src/site.config.ts` file.

### Page contents

To edit the resume homepage content and design, edit the `src/pages/index.astro` file.

### Page components

To edit page components found site-wide such as the card used in the homepage, edit the files found in the `src/components/` directory.

### Layouts

To edit the base layouts of all pages, edit the `src/layouts/BaseLayout.astro` file.

To edit the layout of a blog article, edit the `src/layouts/BlogPost.astro` file.

### Blog content

To add blog content, insert `.md` files in the `src/content/` directory.

To add images in blog articles, insert a folder in the `src/content/` directory, add both the `.md` and image files into the new folder, and reference the image in your `.md` file.

## Theming

To change the theme colours of the site, edit the `src/styles/app.css` file.

To change the fonts of the site, add your font files into `/public`, add it as a `@font-face` in the `src/styles/app.css` file, as a `fontFamily` in the `tailwind.config.js` file, and apply the new font class to the `body` tag in the `src/layouts/BaseLayout.astro` file.
