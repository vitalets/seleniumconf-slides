# Mocking client-side and server-side API calls with Selenium BiDi

Slidev deck for the Selenium BiDi request mocking talk.

## Run locally

```bash
npm install
npm run dev
```

Open <http://localhost:3030>.

## Structure

- `slides.md` contains deck configuration and slide imports.
- `pages/*.md` contains one slide per markdown file.
- `public/` contains static local assets referenced from slides with leading slash paths.
- `style.css` contains global deck styling.

Slide order is controlled by the import order in `slides.md`, so page filenames can stay semantic when slides are inserted or reordered.
