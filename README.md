# News API Project

A real-time news aggregator using NewsAPI.org

## Setup Instructions

### 1. Get Your API Key
1. Go to [NewsAPI.org](https://newsapi.org/)
2. Sign up for a free account
3. Get your API key from the dashboard

### 2. Configure for Local Development
Create a `.env` file in the root directory:
```
NEWS_API_KEY=your_actual_api_key_here
```

### 3. Deploy to Vercel

#### Option A: Using Vercel Dashboard
1. Go to [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. In Project Settings → Environment Variables, add:
   - Key: `NEWS_API_KEY`
   - Value: Your API key from NewsAPI.org
4. Deploy

#### Option B: Using Vercel CLI
```bash
# Install Vercel CLI
npm i -g vercel

# Login
vercel login

# Add environment variable
vercel env add NEWS_API_KEY

# Deploy
vercel --prod
```

## API Endpoint
Once deployed, your API will be available at:
- `/api/news` - Get top headlines
- `/api/news?category=technology` - Get news by category
- `/api/news?country=us` - Get news by country

## Categories
- general
- business
- technology
- sports
- entertainment
- health
- science

## Countries
Use ISO 3166-1 alpha-2 country codes (us, gb, in, etc.)
