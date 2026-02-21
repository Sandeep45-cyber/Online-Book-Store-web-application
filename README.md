# Online Book Store Web Application

A full-stack web application for buying and selling books, built with Node.js, Express, MongoDB, and Handlebars.

## Features

- User authentication (signup/login)
- Browse books by category
- Search books by name
- Book detail pages
- Cart management and checkout flow
- User order history
- Admin dashboard
- Admin book and admin-user management
- Contact/feedback collection
- Image upload to Cloudinary

## Tech Stack

- Runtime: Node.js
- Server: Express.js
- Database: MongoDB
- Template engine: Handlebars (`hbs`)
- File uploads: Multer
- Image hosting: Cloudinary
- Session management: `express-session`

## Project Structure

```text
Online-Book-Store-web-application/
├── assests/              # Static CSS files (as named in current codebase)
├── config/               # Cloudinary and Multer configuration
├── forms/                # Static HTML forms
├── images/               # Local static images
├── routes/               # Express routers (admin routes)
├── scripts/              # Client-side JS
├── views/                # Handlebars templates
├── docs/                 # Extra project documentation
├── index.js              # Main server entry point
├── package.json
└── README.md
```

## Prerequisites

- Node.js 16+ (recommended)
- npm 8+ (or compatible)
- MongoDB instance
- Cloudinary account

## Environment Variables

Create a `.env` file in the project root:

```env
mongo_url=your_mongodb_connection_string
cloud_name=your_cloudinary_cloud_name
api_key=your_cloudinary_api_key
api_secret=your_cloudinary_api_secret
PORT=8000
```

An example file is provided in `.env.example`.

## Local Setup

1. Clone the repository:

```bash
git clone https://github.com/Sandeep45-cyber/Online-Book-Store-web-application.git
cd Online-Book-Store-web-application
```

2. Install dependencies:

```bash
npm install
```

3. Create `.env` from the example and set real values:

```bash
cp .env.example .env
```

4. Start the app:

```bash
npm start
```

5. Open in browser:

```text
http://localhost:8000
```

## Main Routes

- User app: `/`, `/login`, `/signup`, `/search/:name`, `/category/:category`, `/cart/usercart`
- Admin app: `/admin`, `/adminauth`, `/dashboard`, `/orders`, `/adminusers`

Detailed route reference is documented in `docs/ROUTES.md`.

## Documentation

- Setup guide: `docs/SETUP.md`
- Route reference: `docs/ROUTES.md`

## Notes

- Static directory name is currently `assests` in code and repository. Keep this unchanged unless you also refactor code references.
- This codebase uses older package versions. Consider dependency updates before production deployment.
