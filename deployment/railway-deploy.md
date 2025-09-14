# Railway Deployment Guide

## 🚀 Step-by-Step Railway Deployment

### Prerequisites
- GitHub account
- Your project pushed to GitHub

### Step 1: Prepare Your Repository
Make sure these files are in your root directory:
- ✅ `movie_recommender.py`
- ✅ `requirements.txt`
- ✅ `final_dataset.csv`
- ✅ `templates/` folder
- ✅ `static/` folder

### Step 2: Deploy on Railway

1. **Go to Railway:**
   - Visit [railway.app](https://railway.app)
   - Click "Start a New Project"

2. **Connect GitHub:**
   - Click "Deploy from GitHub repo"
   - Authorize Railway to access your GitHub
   - Select your repository

3. **Configure Deployment:**
   - Railway will auto-detect it's a Python app
   - It will automatically find `requirements.txt`
   - No additional configuration needed!

4. **Deploy:**
   - Click "Deploy Now"
   - Wait 2-3 minutes for deployment
   - Your app will be live!

### Step 3: Access Your App
- Railway will provide a URL like: `https://your-app-name.railway.app`
- Click the URL to access your Movie Recommendation System

## 🔧 Railway Configuration

Railway automatically detects:
- **Build Command:** `pip install -r requirements.txt`
- **Start Command:** `python movie_recommender.py`
- **Port:** Automatically assigned

## 📊 Monitoring

- **Logs:** View real-time logs in Railway dashboard
- **Metrics:** Monitor CPU, memory usage
- **Deployments:** Automatic deployments on Git push

## 💰 Pricing

- **Free Tier:** 500 hours/month, 1GB RAM
- **Pro Tier:** $5/month for unlimited usage

## 🐛 Troubleshooting

**If deployment fails:**
1. Check Railway logs for errors
2. Ensure `final_dataset.csv` is in repository
3. Verify `requirements.txt` has all dependencies
4. Check that all files are committed to Git

**If app doesn't work:**
1. Check the logs in Railway dashboard
2. Verify the app starts locally first
3. Check that the CSV file is accessible

## 🔄 Updates

To update your deployed app:
1. Make changes to your code
2. Commit and push to GitHub
3. Railway automatically redeploys!

## 📱 Features Available

✅ Movie search functionality
✅ Genre-based recommendations  
✅ Beautiful UI with dark/light mode
✅ Mobile responsive design
✅ Recommendation button for similar movies
✅ Movie detail pages

---

**Your Movie Recommendation System is now live on the internet!** 🌐
