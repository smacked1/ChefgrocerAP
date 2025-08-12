# AI-Powered Smart Cooking Assistant

## Overview
This full-stack React application is an AI-powered cooking assistant designed to offer an intuitive, hands-free cooking experience. It leverages AI for personalized assistance, streamlines recipe management, meal planning, grocery lists, and pantry inventory, and integrates comprehensive payment processing for premium features. The vision is to simplify home cooking and grocery shopping, saving users time and money, with ambitions for significant market potential and revenue generation through a robust business model.

## User Preferences
- Preferred communication style: Simple, everyday language
- Owner: Myles Barber (dxmylesx22@gmail.com)
- Business: ChefGrocer, 1619 Mound Street, Davenport, IA 52803

## System Architecture

The application follows a monorepo structure separating client and server code.

### Frontend
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter
- **State Management**: TanStack Query (React Query)
- **UI Library**: Radix UI components with shadcn/ui styling
- **Styling**: Tailwind CSS with CSS variables
- **Build Tool**: Vite

### Backend
- **Runtime**: Node.js with Express.js
- **Database**: PostgreSQL with Drizzle ORM (Neon Database for serverless)
- **Authentication**: Replit Auth with OpenID Connect, session management with PostgreSQL storage
- **API Design**: RESTful APIs with JSON responses, protected routes with authentication middleware
- **AI Integration**: Google Gemini AI for voice processing and meal planning
- **Payment Processing**: Stripe integration with user subscription tracking

### Voice Integration
- **Speech Recognition**: Web Speech API with real-time transcription
- **Speech Synthesis**: Web Speech Synthesis API for audio feedback
- **Voice Processing**: Google Gemini AI for natural language understanding, ingredient analysis, and nutrition data extraction
- **Voice-Activated Search**: Hands-free ingredient search with detailed nutrition, allergen warnings, and price estimates.

### Store Location Integration
- **OpenStreetMap Integration**: Real-time nearby store discovery using Nominatim geocoding API
- **Overpass API**: Authentic grocery store, supermarket, and convenience store data with exact locations, addresses, and details
- **Distance Calculations**: Haversine formula for accurate distance measurements in kilometers
- **Store Filtering**: Dynamic search and filtering by store name or brand

### Key Features
- **Voice Commands**: Natural language processing for hands-free interaction.
- **Recipe Management**: Create, search, and manage recipes with nutrition analysis.
- **Meal Planning**: AI-assisted generation based on preferences.
- **Smart Shopping**: Enhanced grocery lists with real-time price comparison, savings, and authentic nearby store locations via OpenStreetMap.
- **Nutrition Tracking**: Comprehensive analysis for recipes and ingredients.
- **Payment Processing**: Secure Stripe integration for one-time purchases and monthly/yearly subscriptions, including a Lifetime Pass option.
- **Subscription Management**: Multiple tiers (Free, Premium, Pro, Lifetime) with feature differentiation.
- **Privacy Compliance System**: Complete privacy policy implementation with GDPR/CCPA compliance, user data control, and cookie consent management.
- **Business Scaling Features**: Restaurant partnership portal, affiliate revenue tracking, premium content marketplace, and usage analytics dashboard.

## External Dependencies

### Core
- **@neondatabase/serverless**: Serverless PostgreSQL database connection.
- **drizzle-orm**: Type-safe database ORM.
- **@tanstack/react-query**: Server state management.
- **@google/genai**: Google Gemini AI integration for various AI functionalities.
- **Spoonacular API**: Premium recipe and nutrition API.
- **TheMealDB API**: Free recipe database.
- **USDA FoodData Central API**: Official USDA nutrition database.

### UI
- **@radix-ui/***: Accessible UI component primitives.
- **tailwindcss**: Utility-first CSS framework.
- **lucide-react**: Icon library.

### Voice
- **Web Speech API**: Browser-native speech recognition.
- **Web Speech Synthesis API**: Browser-native text-to-speech.

### Mobile Deployment
- **@capacitor/core**: Native mobile app wrapper for iOS and Android.
- **@capacitor/ios**: iOS platform integration for App Store deployment.
- **@capacitor/assets**: Automated app icon and splash screen generation.