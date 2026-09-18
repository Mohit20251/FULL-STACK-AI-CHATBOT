# QuickGPT — Full Stack AI Chatbot

A full-stack AI chatbot application built with React, Node.js, MongoDB, and the Gemini API. Includes user authentication, chat history, image uploads via ImageKit, and credit-based payments via Stripe.

---

## Tech Stack

**Frontend:** React 19, Vite, Tailwind CSS v4, React Router, Axios  
**Backend:** Node.js, Express 5, MongoDB (Mongoose), JWT  
**Services:** Google Gemini API, ImageKit, Stripe

---

## Project Structure

```
QuickGPT/
├── client/       # React frontend
└── server/       # Express backend
```

---

## Getting Started

### Prerequisites

- Node.js v18+
- MongoDB database (local or Atlas)
- Accounts for: [Gemini API](https://aistudio.google.com/), [ImageKit](https://imagekit.io/), [Stripe](https://stripe.com/)

---

### 1. Clone the repo

```bash
git clone https://github.com/Mohit20251/FULL-STACK-AI-CHATBOT.git
cd FULL-STACK-AI-CHATBOT/QuickGPT
```

### 2. Setup the Server

```bash
cd server
npm install
```

Create a `.env` file in `server/` (see `.env.example`), then:

```bash
npm run server
```

Server runs on `http://localhost:3000`

### 3. Setup the Client

```bash
cd client
npm install
```

Create a `.env` file in `client/` (see `.env.example`), then:

```bash
npm run dev
```

Client runs on `http://localhost:5173`

---

## Environment Variables

### `server/.env`

| Variable | Description |
|---|---|
| `JWT_SECRET` | Secret key for signing JWTs |
| `MONGODB_URI` | MongoDB connection string |
| `GEMINI_API_KEY` | Google Gemini API key |
| `IMAGEKIT_PUBLIC_KEY` | ImageKit public key |
| `IMAGEKIT_PRIVATE_KEY` | ImageKit private key |
| `IMAGEKIT_URL_ENDPOINT` | ImageKit URL endpoint |
| `STRIPE_PUBLISHABLE_KEY` | Stripe publishable key |
| `STRIPE_SECRET_KEY` | Stripe secret key |
| `STRIPE_WEBHOOK_SECRET` | Stripe webhook signing secret |

### `client/.env`

| Variable | Description |
|---|---|
| `VITE_SERVER_URL` | Backend API URL (default: `http://localhost:3000`) |

---

## Deployment

Both `client/` and `server/` include a `vercel.json` for easy deployment on [Vercel](https://vercel.com/).

- Deploy `server/` as a separate Vercel project
- Deploy `client/` as a separate Vercel project
- Set `VITE_SERVER_URL` in the client's Vercel environment variables to point to the deployed server URL

---

## Features

- User authentication (JWT)
- Real-time AI chat powered by Gemini
- Chat history with sidebar navigation
- Image upload support via ImageKit
- Credit system with Stripe payments
- Dark mode support
- Community page
- Responsive design

---

## License

MIT
