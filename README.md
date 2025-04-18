# AI Car Marketplace 🚗

A modern full-stack car marketplace application built with Next.js, featuring AI-powered search, test drive booking, and admin dashboard.

![Vehiql Screenshot](https://github.com/user-attachments/assets/dee04576-f30e-4ab8-af7d-f4633621379c)

## Features 🌟

- AI-powered image search using Google's Gemini API
- User authentication with Clerk
- Real-time car listings with Supabase
- Test drive booking system
- Admin dashboard for car management
- Responsive design with Tailwind CSS
- Modern UI components with Shadcn UI
- Rate limiting and bot protection with ArcJet

## Tech Stack 💻

- **Frontend**: Next.js 14, React 19, Tailwind CSS
- **Backend**: Next.js API Routes, Prisma ORM
- **Database**: PostgreSQL (via Supabase)
- **Authentication**: Clerk
- **AI**: Google Gemini API
- **UI Components**: Shadcn UI
- **Security**: ArcJet
- **Styling**: Tailwind CSS

## Getting Started 🚀

### Prerequisites

- Node.js 18+ 
- PostgreSQL database 
- Clerk account
- Google Gemini API key
- ArcJet account

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-car-marketplace.git
cd ai-car-marketplace
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with the following variables:
```env
DATABASE_URL=your_database_url
DIRECT_URL=your_direct_url

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_pub_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=your_gemini_api_key

ARCJET_KEY=your_arcjet_key
```

4. Run database migrations:
```bash
npx prisma migrate dev
```

5. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Project Structure 📁

```
├── actions/          # Server actions
├── app/             # Next.js app router pages
├── components/      # React components
├── lib/            # Utility functions and configurations
├── prisma/         # Database schema and migrations
└── public/         # Static assets
```

## Key Features Explained 🔑

### AI Image Search
Upload an image of a car, and the system will use Google's Gemini API to identify similar cars in the inventory.

### Test Drive Booking
Users can schedule test drives for available cars, with automatic availability management.

### Admin Dashboard
Comprehensive admin interface for:
- Managing car listings
- Handling test drive bookings
- Viewing analytics
- Configuring dealership settings

## Contributing 🤝

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments 👏

- Built following RoadsideCoder's tutorial
- UI components from Shadcn UI
- Authentication powered by Clerk
- Database hosting by Supabase
