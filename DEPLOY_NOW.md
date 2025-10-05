# Quick Deploy to Vercel

## Your API Key
`ce0f35c908664e329facbce4e5a0b973`

## Deploy Now - 2 Options:

### Option 1: Vercel Dashboard (Easiest - 2 minutes)

1. **Go to Vercel**: https://vercel.com/login
   - Sign in with GitHub

2. **Import Project**:
   - Click "Add New..." → "Project"
   - Select `samarpithmenezes32/news-api`
   - Click "Import"

3. **Add Environment Variable**:
   - In the import screen, expand "Environment Variables"
   - Add:
     - Name: `NEWS_API_KEY`
     - Value: `ce0f35c908664e329facbce4e5a0b973`
   - Click "Add"

4. **Deploy**:
   - Click "Deploy"
   - Wait ~1 minute
   - ✅ Done!

### Option 2: Using Vercel CLI

Open PowerShell and run these commands:

```powershell
# Install Vercel CLI (one time only)
npm install -g vercel

# Go to your project
cd "c:\Users\Samarpith\Downloads\news api-20251005T141005Z-1-001\news api"

# Login to Vercel
vercel login

# Deploy (it will ask for the API key)
vercel

# When asked for environment variables, add:
# NEWS_API_KEY = ce0f35c908664e329facbce4e5a0b973

# Deploy to production
vercel --prod
```

## After Deployment

Your news site will be live at a URL like:
- `https://news-api-xyz.vercel.app`

The site will show:
- ✅ Real news from around the world
- ✅ Images with articles
- ✅ Working category filters
- ✅ Links to full articles
- ✅ Auto-refresh every 5 minutes

## No More 404 Error! 🎉

The API key is now configured and your site will work perfectly.
