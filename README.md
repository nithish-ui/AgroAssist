
# Farm Assistant

Farm Assistant is a complete full-stack web application designed to help farmers make data-driven decisions for improved crop yields and sustainable farming practices.

## Features

- **Crop Recommendation**: Get personalized crop recommendations based on soil type, location, and season
- **Fertilizer Guide**: Discover the best fertilizers for specific crops and soil conditions
- **Weather Report**: Access real-time weather data and forecasts tailored for agricultural needs
- **Market Prices**: Track current market prices for various crops to optimize selling decisions
- **Agricultural Chatbot**: Ask questions and get intelligent answers about farming practices and challenges

## Technologies Used

- **Frontend**: React with TypeScript
- **Styling**: Tailwind CSS with shadcn/ui components
- **Backend**: Supabase for authentication and database
- **AI Integration**: OpenAI (for crop and fertilizer recommendations) and Google Gemini (for weather and chatbot)

## Setup Instructions

1. Clone the repository
```bash
git clone <repository-url>
cd farm-assistant
```

2. Install dependencies
```bash
npm install
```

3. Start the development server
```bash
npm run dev
```

4. Open the application in your browser
```
http://localhost:8080
```

## Environment Variables

The application uses the following environment variables:

```
# Supabase Configuration
NEXT_PUBLIC_SUPABASE_URL=https://kfkpvcipjixdilvslzwt.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imtma3B2Y2lwaml4ZGlsdnNsend0Iiwicm9sZSI6ImFub24iLCJpYXQiOjE3NDUwMTM0OTUsImV4cCI6MjA2MDU4OTQ5NX0._TkvEPSK_dvRmGm0Wtuc8K9NYt3NBtw58t12J6f3lE0
DATABASE_URL=postgresql://postgres:agrislove@123@db.kfkpvcipjixdilvslzwt.supabase.co:5432/postgres

# API Keys
OPENAI_API_KEY=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
GEMINI_API_KEY=AIzaSyBCbcPRwAROEh4gYF-vS_kVIAaeIdYw49U
```

These are managed through the `src/lib/env.ts` file.

## Database Schema

The Supabase database includes the following tables:

- `crops`: Information about different crop types
- `fertilizer_suggestions`: Recommended fertilizers based on crops and soil
- `weather_logs`: Weather data history
- `market_prices`: Current and historical crop prices
- `users`: User authentication and profile data
- `chat_logs`: Record of user conversations with the chatbot

## Deployment

This application is ready to be deployed on platforms like Vercel, Netlify, or any hosting service that supports React applications.

## License

This project is licensed under the MIT License.
