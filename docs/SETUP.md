# Setup Guide

## 1. Prerequisites

- Node.js 16+ recommended
- npm 8+ recommended
- MongoDB running locally or remotely
- Cloudinary account for image uploads

## 2. Install Dependencies

```bash
npm install
```

## 3. Configure Environment

Copy `.env.example` to `.env` and fill in your values:

```bash
cp .env.example .env
```

Required variables:

- `mongo_url`: MongoDB connection string
- `cloud_name`: Cloudinary cloud name
- `api_key`: Cloudinary API key
- `api_secret`: Cloudinary API secret
- `PORT`: Server port (defaults to `8000`)

## 4. Run the Application

```bash
npm start
```

Visit:

```text
http://localhost:8000
```

## 5. Minimum Database Collections

The app expects these collections in MongoDB database `schema`:

- `users`
- `bookdetails`
- `admin`
- `sell`
- `contactinfo`

## 6. Optional Initial Data

To access admin dashboard, create at least one `admin` document in MongoDB:

```json
{
  "username": "admin",
  "password": "admin123",
  "name": "Admin User",
  "emailid": "admin@example.com"
}
```

## 7. Troubleshooting

- If login or dashboard fails, verify MongoDB connection and collection names.
- If book image uploads fail, verify Cloudinary credentials in `.env`.
- If static files do not load, confirm folder name is exactly `assests` (current project spelling).
