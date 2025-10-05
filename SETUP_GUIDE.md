# 🔑 HOW TO GET YOUR NEWS API KEY AND DEPLOY

## Step 1: Get Your Free API Key

1. **Go to NewsAPI.org**
   - Visit: https://newsapi.org/
   
2. **Sign Up (Free)**
   - Click "Get API Key" button
   - Fill in your details
   - Verify your email
   
3. **Copy Your API Key**
   - After login, go to your account dashboard
   - Copy the API key (it looks like: `abc123def456...`)

## Step 2: Deploy to Vercel

### Option A: Vercel Dashboard (Recommended - Easiest)

1. **Go to Vercel**
   - Visit: https://vercel.com
   - Sign in with GitHub

2. **Import Your Project**
   - Click "New Project"
   - Find and select `samarpithmenezes32/news-api`
   - Click "Import"

3. **Add Environment Variable**
   - Before deploying, click "Environment Variables"
   - Add:
     - **Name**: `NEWS_API_KEY`
     - **Value**: (paste your API key from NewsAPI.org)
   - Click "Add"

4. **Deploy**
   - Click "Deploy"
   - Wait 1-2 minutes
   - Done! Your site will be live!

### Option B: Vercel CLI

```powershell
# Install Vercel CLI
npm i -g vercel

# Navigate to your project
cd "c:\Users\Samarpith\Downloads\news api-20251005T141005Z-1-001\news api"

# Login to Vercel
vercel login

# Add your API key
vercel env add NEWS_API_KEY
# When prompted, paste your API key

# Deploy
vercel --prod
```

## Step 3: Verify It Works

After deployment, visit your Vercel URL. You should see:
- Real news articles with images
- Working category filters
- "Read more" links to full articles

## Troubleshooting

**Still getting 404?**
- Make sure you added the `NEWS_API_KEY` environment variable
- Redeploy after adding the environment variable

**No news showing?**
- Check browser console (F12) for errors
- Verify your API key is valid at https://newsapi.org/account

**API limit exceeded?**
- Free tier: 100 requests/day
- Consider upgrading or caching results

## Free Tier Limits
- ✅ 100 requests per day
- ✅ Top headlines
- ✅ Multiple categories
- ❌ Historical data (paid only)
