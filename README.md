# E-COMMERCE-SHOPPING

A full-stack e-commerce shopping application built with React (Vite) frontend and Node.js/Express backend with MongoDB.

## Project Structure

```
E-COMMERCE-SHOPPING/
├── Frontend/          # React + Vite frontend application
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── hooks/       # Custom React hooks
│   │   ├── images/      # Static image assets
│   │   ├── pages/       # Page components
│   │   ├── store/       # Redux store configuration
│   │   └── utils/       # Utility functions
│   ├── public/
│   ├── App.jsx
│   ├── index.html
│   ├── package.json
│   ├── vite.config.js
│   └── tailwind.config.js
│
├── Server/            # Node.js + Express backend API
│   ├── controllers/    # Route controllers
│   ├── database/       # Database configuration
│   ├── middlewares/    # Express middlewares
│   ├── models/         # Mongoose models
│   ├── routes/         # API route definitions
│   ├── utils/          # Helper utilities
│   ├── app.js          # Express app setup
│   ├── index.js        # Entry point
│   └── package.json
│
└── README.md
```

## Tech Stack

**Frontend:**
- React 18 + Vite
- Redux Toolkit (state management)
- Tailwind CSS + Flowbite (styling)
- Axios (HTTP client)
- Font Awesome / React Icons
- React Router DOM

**Backend:**
- Node.js + Express
- MongoDB + Mongoose
- JWT Authentication
- Passport (Google OAuth)
- Cloudinary (media upload)
- Multer (file upload)
- bcrypt (password hashing)

## Getting Started

### Prerequisites
- Node.js (v16+)
- MongoDB
- npm or yarn

### Installation & Setup

**1. Clone the repository**
```bash
git clone https://github.com/Manu11223/E-COMMERCE-SHOPPING.git
cd E-COMMERCE-SHOPPING
```

**2. Install Backend Dependencies**
```bash
cd Server
npm install
```

**3. Configure Environment Variables**
```bash
# Create a .env file in the Server directory with:
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

**4. Install Frontend Dependencies**
```bash
cd ../Frontend
npm install
```

**5. Run the Application**

Start the backend server:
```bash
cd Server
npm run dev
```

Start the frontend dev server (in a new terminal):
```bash
cd Frontend
npm run dev
```

The frontend will be available at `http://localhost:5173` and the backend API at `http://localhost:5000`.

## Available Scripts

### Frontend
| Command | Description |
|---------|-------------|
| `npm run dev` | Start Vite dev server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

### Backend
| Command | Description |
|---------|-------------|
| `npm run dev` | Start with nodemon (hot reload) |
| `npm start` | Start server |
