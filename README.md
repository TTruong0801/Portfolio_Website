# Portfolio_Website

A personal portfolio website for Thien Truong. Visitors can browse my projects, and after logging in I can add, edit, and delete them.

## Live Demo
- Deployed app: [(https://gleeful-haupia-161590.netlify.app/)](https://thientruongportfolio.netlify.app/)
- Demo video (unlisted): (https://youtu.be/gZMr7Se-H1k)

## What It Does
- Displays my projects, About section, and contact info
- User registration, login, and logout (Supabase Auth)
- Logged-in users can create, edit, and delete projects (full CRUD)
- Projects are stored in a Supabase database, and row-level security ensures only the owner can modify their own entries

## Technologies Used
- HTML, CSS, and JavaScript (single-page `index.html`)
- Supabase (Postgres database and authentication)
- GitHub (version control)
- Netlify (hosting)
- AI tools used during development: Claude

## Setup Instructions
1. Clone or download this repository.
2. Create a free project at [supabase.com](https://supabase.com).
3. In the Supabase SQL Editor, create the `projects` table with row-level security (table columns: `id`, `user_id`, `title`, `description`, `tech`, `link`, `created_at`).
4. In `index.html`, set `SUPABASE_URL` and `SUPABASE_ANON_KEY` to your project's URL and publishable key.
5. Open `index.html` in a browser, or deploy the repo to Netlify.

## Project Structure
- `index.html`: the entire app (layout, styling, and Supabase logic)
- `README.md`: project documentation
