# HOLLA TRAVEL - Bangladesh Travel Booking SaaS

A premium travel booking platform for Bangladesh with AI-powered trip planning, real-time hotel bookings, and Firebase backend.

## 🚀 Features

- **AI Travel Planner**: GPT-4o powered intelligent trip planning
- **Real Authentication**: Firebase Auth with secure user management
- **Hotel Booking System**: Dynamic hotel listings with real-time data
- **Firebase Backend**: Firestore database for scalable data management
- **Premium UI**: Modern dark theme with smooth animations
- **Mobile Responsive**: Optimized for all devices
- **Zero-Cost Startup**: Built with free tiers of Firebase and OpenAI

## 🛠️ Tech Stack

- **Frontend**: Next.js 14 (App Router), React 18, Tailwind CSS
- **Backend**: Firebase (Auth + Firestore), Next.js API Routes
- **AI**: OpenAI GPT-4o-mini for travel planning
- **Animations**: Framer Motion
- **Deployment**: Vercel (recommended)

## 📋 Prerequisites

- Node.js 18+
- npm or yarn
- Firebase account
- OpenAI API account

## ⚡ Quick Start

### 1. Clone & Install

```bash
git clone <your-repo-url>
cd holla-travel
npm install
```

### 2. Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a new project
3. Enable Authentication and Firestore Database
4. Get your Firebase config values

### 3. OpenAI Setup

1. Go to [OpenAI Platform](https://platform.openai.com)
2. Create an API key
3. Note down your API key

### 4. Environment Variables

```bash
cp .env.example .env.local
```

Update `.env.local` with your actual values:

```env
# Firebase Config
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

# OpenAI Config
OPENAI_API_KEY=your_openai_api_key
```

### 5. Seed Database

1. Start the development server: `npm run dev`
2. Go to `/admin` page
3. Click "🌱 Seed Database" to populate with sample hotels

### 6. Development

```bash
npm run dev
```

Visit `http://localhost:3000`

## 📁 Project Structure

```
holla-travel/
├── app/                    # Next.js App Router
│   ├── admin/             # Admin dashboard
│   ├── ai-planner/        # AI travel planning
│   ├── api/               # API routes
│   ├── auth/              # Authentication
│   ├── booking/           # Hotel listings
│   └── ...
├── components/            # Reusable components
├── lib/                   # Firebase config & services
├── scripts/               # Utility scripts
└── public/                # Static assets
```

## 🔧 API Routes

- `POST /api/ai` - AI travel planning
- `POST /api/auth/signup` - User registration
- `POST /api/auth/login` - User login

## 🗄️ Database Schema

### Hotels Collection
```javascript
{
  name: "Hotel Name",
  location: "City, Bangladesh",
  rating: 5,
  price: 4500,
  type: "Hotel",
  category: "luxury",
  amenities: ["WiFi", "AC", "Pool"],
  description: "Hotel description",
  image: "🏨",
  active: true,
  createdAt: Timestamp
}
```

### Bookings Collection
```javascript
{
  userId: "firebase_uid",
  hotelId: "hotel_doc_id",
  checkIn: "2024-01-15",
  checkOut: "2024-01-17",
  guests: 2,
  totalAmount: 9000,
  status: "confirmed",
  createdAt: Timestamp
}
```

## 🚀 Deployment

### Vercel (Recommended)

1. Push to GitHub
2. Connect to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy!

### Manual Build

```bash
npm run build
npm start
```

## 💰 Cost Structure (Free Tier)

- **Firebase**: 1GB database, 50K reads/day, 20K writes/day
- **OpenAI**: $5 free credits, then $0.002/1K tokens
- **Vercel**: 100GB bandwidth, custom domain free
- **Total Monthly Cost**: $0-5 (depending on usage)

## 🔒 Security

- Firebase Authentication for secure user management
- Environment variables for API keys
- Server-side API validation
- CORS protection

## 📱 Features Overview

### AI Travel Planner
- Natural language trip planning
- Bangladesh-focused recommendations
- Personalized itineraries
- Budget optimization

### Hotel Booking
- Real-time hotel search
- Location-based filtering
- Price range selection
- Instant booking confirmation

### Admin Dashboard
- Hotel management
- Booking analytics
- User management
- Revenue tracking

## 🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## 📄 License

MIT License - feel free to use for your own projects!

## 🆘 Support

- Email: hello@holla.com
- Issues: GitHub Issues
- Docs: This README

---

**Built with ❤️ for Bangladesh travelers**
   ```bash
   npm install
   ```

3. **Start development server:**
   ```bash
   npm run dev
   ```

4. **Open in browser:**
   ```
   http://localhost:3000
   ```

---

## 🛠️ Development

### Available Scripts

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Run linting
npm run lint
```

---

## 📁 Project Structure

```
holla/
├── app/
│   ├── layout.js           # Root layout with metadata
│   ├── page.js             # Home page
│   ├── globals.css         # Global styles
│   ├── about/
│   │   └── page.js         # About page
│   ├── services/
│   │   └── page.js         # Services page
│   ├── portfolio/
│   │   └── page.js         # Portfolio page
│   └── contact/
│       └── page.js         # Contact page
├── components/
│   ├── Navbar.jsx          # Navigation bar
│   └── Chatbot.jsx         # Live chat widget
├── package.json            # Dependencies
├── next.config.js          # Next.js configuration
├── tailwind.config.js      # Tailwind CSS config
├── postcss.config.js       # PostCSS config
└── .eslintrc.json          # ESLint config
```

---

## 🎨 Design System

### Color Palette
- **Primary**: Black (#000000)
- **Secondary**: White (#FFFFFF)
- **Accent**: Neon Blue (#3B82F6) / Purple (#8B5CF6)
- **Background**: Charcoal grays

### Typography
- **Font Family**: Inter, Poppins (Google Fonts)
- **Font Weights**: 400, 500, 600, 700

### Animation
- Powered by **Framer Motion**
- Smooth transitions and micro-interactions
- Viewport-triggered animations

---

## 🔧 Technologies Used

- **Framework**: Next.js 14
- **React**: 18
- **Styling**: Tailwind CSS 3
- **Animations**: Framer Motion 10
- **Language**: JavaScript/JSX
- **Build Tool**: Next.js build system
- **Linting**: ESLint

---

## 📊 Performance

- Fast page loads with Next.js optimization
- Image optimization
- Code splitting
- CSS optimization via Tailwind
- Mobile responsiveness

---

## 🌐 Branding

**Company Identity:**
- Brand Name: **Holla**
- Tagline: "Engineering Perception. Building Desire."
- Positioning: Premium, innovative, luxury digital experiences
- Sister Company: Rasits Inc.

**Branding Elements:**
- Logo: "HOLLA" wordmark (minimal sans-serif)
- Footer Note: "© All Rights Reserved by Rasits Inc."
- Throughout: "A Sister Concern of Rasits Inc."

---

## 📝 Environment Configuration

Create a `.env.local` file for environment variables:

```env
NEXT_PUBLIC_SITE_NAME=Holla
NEXT_PUBLIC_CONTACT_EMAIL=hello@holla.com
NEXT_PUBLIC_PHONE=+1 (555) 123-4567
```

See `.env.example` for more details.

---

## 🚀 Deployment

### Build for Production
```bash
npm run build
npm start
```

### Deployment Platforms
- **Vercel** (Recommended for Next.js)
- **Netlify**
- **AWS Amplify**
- **Any Node.js hosting**

---

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

---

## 👥 Components

### Navbar
Fixed navigation bar with logo and page links. Implements glassmorphism with backdrop blur.

### Chatbot
Floating chat widget for user engagement. Expandable interface with smooth animations.

### Hero Section
Large, eye-catching section with gradient text and CTA buttons.

### Feature Cards
Reusable card components with hover effects and animations.

### Forms
Validated contact form with success feedback and email integration.

---

## 🔐 Security

- HTTPS ready for production
- Form validation on client-side
- CSRF protection (Next.js built-in)
- No sensitive data in frontend code

---

## 📞 Support & Contact

For inquiries about the Holla brand, visit:
- **Email**: hello@holla.com
- **Phone**: +1 (555) 123-4567

---

## 📄 License

© All Rights Reserved by Rasits Inc.

---

**Built with ❤️ using Next.js, React, and Tailwind CSS**