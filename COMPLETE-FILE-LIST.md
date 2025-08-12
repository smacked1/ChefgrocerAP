# ChefGrocer - Complete File Structure for Freelancer Testing

## Core Application Files

### Package Configuration
- `package.json` - Dependencies and scripts
- `package-lock.json` - Locked dependency versions
- `tsconfig.json` - TypeScript configuration
- `vite.config.ts` - Build tool configuration
- `tailwind.config.ts` - Styling configuration
- `postcss.config.js` - CSS processing
- `components.json` - UI components config

### Environment & Deployment
- `.env` - Environment variables (create with secrets)
- `.replit` - Replit configuration
- `replit.md` - Project documentation
- `drizzle.config.ts` - Database configuration

### Frontend (client/)
- `client/src/App.tsx` - Main React app
- `client/src/main.tsx` - App entry point
- `client/src/index.css` - Global styles

#### Components (client/src/components/)
- `ui/` - Shadcn UI components
- `promotional-banner.tsx` - Revenue banner
- `revenue-booster.tsx` - Conversion optimizer
- `voice-assistant.tsx` - Voice command interface

#### Pages (client/src/pages/)
- `Home.tsx` - Main dashboard
- `Landing.tsx` - Landing page
- `Subscribe.tsx` - Subscription plans
- `Checkout.tsx` - Payment processing
- `Revenue.tsx` - Revenue dashboard
- `RevenueOptimization.tsx` - Analytics
- `NotFound.tsx` - 404 page

#### Hooks & Utils (client/src/)
- `hooks/useAuth.ts` - Authentication
- `hooks/use-toast.ts` - Notifications
- `lib/queryClient.ts` - API client
- `lib/utils.ts` - Utilities

### Backend (server/)
- `server/index.ts` - Express server entry
- `server/routes.ts` - API endpoints
- `server/storage.ts` - Database operations
- `server/replitAuth.ts` - Authentication
- `server/db.ts` - Database connection
- `server/vite.ts` - Vite integration

### Database Schema
- `shared/schema.ts` - Drizzle database schema

### Mobile App (iOS/Android)
- `capacitor.config.ts` - Mobile configuration
- `app.json` - App metadata
- `eas.json` - Expo build config

### Documentation Files
- `FREELANCER-TESTING-GUIDE.md` - Testing instructions
- `MULTI-PLATFORM-DEPLOYMENT.md` - Deployment strategy
- `social-media-launch.md` - Marketing content
- `DEPLOYMENT-READY.md` - Production checklist
- `PROJECT-STATUS.md` - Current status
- `iOS-DEPLOYMENT.md` - iOS app instructions
- Various other .md files with strategy docs

## Critical Files for Testing

### Must Have:
1. `package.json` - Install dependencies
2. `server/index.ts` - Start server
3. `client/src/App.tsx` - Main app
4. `shared/schema.ts` - Database structure
5. `server/routes.ts` - API endpoints
6. `.env` - Environment variables (you create)

### Environment Variables Needed:
```env
VITE_STRIPE_PUBLIC_KEY=pk_test_...
STRIPE_SECRET_KEY=sk_test_...
GEMINI_API_KEY=...
DATABASE_URL=postgresql://...
SESSION_SECRET=random_secret_here
```

### Key Features to Test:
- Voice commands (microphone permission required)
- Payment processing (Stripe test mode)
- AI meal planning (Google Gemini)
- User authentication
- Revenue optimization dashboard

## Setup Instructions for Freelancer

1. Download all project files
2. Run `npm install` 
3. Create `.env` with required variables
4. Run `npm run dev`
5. Test at http://localhost:5000

The app is production-ready with working payments, voice AI, and revenue optimization features.