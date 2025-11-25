# Mentora – Your Personal Mentor Booking Platform  
Live Demo: https://mentora-live.netlify.app/

A full-stack, production-ready mentorship platform that connects aspiring professionals (mentees) with experienced mentors. Book 1-on-1 sessions, pay securely, manage availability, and build a stunning public mentor profile – all in one place.

**Built to impress recruiters** – clean architecture, modern tech stack, authentication with refresh tokens, secure payments, cloud uploads, responsive UI, and real-time deployment.

Perfect first big project for junior developers who want to learn how real-world apps are built.

## Features That Stand Out

| Feature                        | What It Does                                                                 | Tech Used                              |
|--------------------------------|------------------------------------------------------------------------------|----------------------------------------|
| Dual User Roles                | Separate experiences for Mentors & Mentees                                   | React Context + Protected Routes       |
| Secure Authentication         | JWT + HttpOnly refresh tokens + automatic token refresh                     | bcrypt, jsonwebtoken, axios interceptors |
| Mentor Profile Builder         | Step-by-step wizard (Personal → Work → Education → Expertise → Rate → Availability) | React Router, Multi-step Form          |
| Cloud Avatar Upload            | Drag-and-drop profile pictures stored on Cloudinary                          | Multer + Cloudinary                    |
| Razorpay Payment Integration   | Real Indian payment gateway (test & live mode ready)                         | Razorpay Node.js SDK                   |
| Responsive & Beautiful UI      | Glassmorphism cards, animations, dark-mode-ready                            | Tailwind CSS + Framer Motion + Lucide icons |
| Availability Calendar          | Weekly recurring slots with time picker                                      | Custom React component                 |
| Real-time Notifications       | Skeleton for future push/email notifications                                | Ready structure                        |
| Production-Grade Deployment    | Frontend on Netlify • Backend on Render • Automatic CI/CD                   | Vite + Express                        |

## Tech Stack (Modern & In-Demand 2025)

### Frontend
- React 19 + Vite (fast dev server & optimized builds)
- React Router v7
- Tailwind CSS v4
- Framer Motion (smooth animations)
- Lucide React icons
- Axios + interceptors for token refresh
- Context API for global auth state

### Backend
- Node.js + Express
- MongoDB Atlas + Mongoose ODM
- JWT authentication with refresh tokens
- Cloudinary for image storage
- Razorpay for payments
- CORS + HttpOnly cookies (secure in production)

### DevOps & Tools
- Git + GitHub
- Netlify (frontend) – zero-config builds
- Render.com (backend) – free tier with custom domain support
- ESLint + Prettier
- Environment variables management

## How to Run Locally

### 1. Clone the repo
```bash
git clone https://github.com/your-username/mentora.git
cd mentora
```

### 2. Backend Setup
```bash
cd backend
cp .env.example .env        # then fill your own keys
npm install
npm run dev                 # starts on http://localhost:3000
```

Required (free tier works):
- MongoDB Atlas cluster
- Cloudinary account
- Razorpay test keys

### 3. Frontend Setup
```bash
cd ../frontend
cp .env.example .env
# Edit .env → VITE_API_BASE_URL=http://localhost:3000/api
npm install
npm run dev                 # opens http://localhost:5173
```


## API Endpoints (Key Ones)

| Method | Endpoint                        | Description                         |
|--------|---------------------------------|-------------------------------------|
| POST   | `/api/auth/create-user`         | Register new user                   |
| POST   | `/api/auth/login`               | Login → sets HttpOnly cookies       |
| POST   | `/api/auth/refresh-token`       | Automatic access token refresh      |
| PUT    | `/api/profile/update-profile`   | Upload avatar + bio, profession…   |
| POST   | `/api/profile/work-experience`  | Add past jobs                       |
| POST   | `/api/profile/rate`             | Set hourly rate                     |
| POST   | `/api/session/initiate-session` | Create payment order + session      |

## Why Recruiters Like This Project

- Full-stack with user authentication & authorization
- Secure cookie-based JWT flow (industry standard)
- Payment gateway integration (Razorpay = Stripe equivalent in India)
- File uploads to Cloudinary (real-world media handling)
- Multi-step form with progress persistence
- Clean separation of concerns & reusable components
- Production deployment with CI/CD
- Responsive, polished UI that actually feels like a real product

## Future Roadmap (Already Planned)

- Video call integration (Daily.co / Agora)
- Google Calendar sync
- Reviews & ratings system
- Search + filters for mentors
- Email/SMS notifications
- Admin dashboard

Built with love by Nishit Jain – always open to collaboration & feedback!  

connect - https://in.linkedin.com/in/nishitjain23
nishit12345.jain@gmail.com