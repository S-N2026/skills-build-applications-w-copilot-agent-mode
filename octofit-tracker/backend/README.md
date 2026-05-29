# OctoFit Tracker - Backend

Node.js + Express + TypeScript backend API for the OctoFit Tracker project with MongoDB integration via Mongoose.

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- MongoDB (local or Atlas)

### Installation

```bash
cd octofit-tracker/backend
npm install
```

### Environment Setup

Create a `.env` file from `.env.example`:

```bash
cp .env.example .env
```

Update the `MONGODB_URI` with your MongoDB connection string.

### Development

Start the development server with hot reload:

```bash
npm run dev
```

The API will be available at `http://localhost:5000`.

### Build

Build for production:

```bash
npm run build
```

### Start Production

```bash
npm start
```

## Project Structure

```
src/
├── index.ts          # Entry point
├── models/           # Mongoose schemas
│   └── User.ts       # User model
├── routes/           # API routes
├── controllers/      # Route handlers
└── middleware/       # Custom middleware
```

## Technologies

- **Express** - Web framework
- **TypeScript** - Type safety
- **Mongoose** - MongoDB ODM
- **CORS** - Cross-origin requests

## API Endpoints

### Health Check
- `GET /api/health` - Check API status

## Environment Variables

- `MONGODB_URI` - MongoDB connection string (default: mongodb://localhost:27017/octofit)
- `PORT` - Server port (default: 5000)
- `NODE_ENV` - Environment (development, production)
