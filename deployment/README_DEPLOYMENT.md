# Movie Recommendation System - Deployment Guide

## 🚀 Quick Deployment Options

### Option 1: Railway (Recommended - Easiest)

1. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Ready for deployment"
   git push origin main
   ```

2. **Deploy on Railway:**
   - Go to [railway.app](https://railway.app)
   - Sign up with GitHub
   - Click "New Project" → "Deploy from GitHub repo"
   - Select your repository
   - Railway will auto-deploy!

3. **Your app will be live at:** `https://your-app-name.railway.app`

---

### Option 2: Render

1. **Push to GitHub** (same as above)

2. **Deploy on Render:**
   - Go to [render.com](https://render.com)
   - Sign up with GitHub
   - Click "New" → "Web Service"
   - Connect your repository
   - Settings:
     - **Build Command:** `pip install -r requirements.txt`
     - **Start Command:** `python movie_recommender.py`
   - Click "Deploy"

3. **Your app will be live at:** `https://your-app-name.onrender.com`

---

### Option 3: Heroku

1. **Install Heroku CLI:**
   - Download from [devcenter.heroku.com](https://devcenter.heroku.com/articles/heroku-cli)

2. **Deploy:**
   ```bash
   # Login to Heroku
   heroku login
   
   # Create app
   heroku create your-movie-app-name
   
   # Deploy
   git add .
   git commit -m "Deploy to Heroku"
   git push heroku main
   ```

3. **Your app will be live at:** `https://your-movie-app-name.herokuapp.com`

---

## 📁 Files Added for Deployment

- `requirements.txt` - Python dependencies
- `Procfile` - Tells Heroku how to run your app
- `runtime.txt` - Specifies Python version
- `.gitignore` - Excludes unnecessary files from Git

## 🔧 Environment Variables

The app automatically uses:
- `PORT` - Set by the hosting platform
- `HOST` - Set to '0.0.0.0' for external access

## 🎯 Features Deployed

✅ Movie search functionality
✅ Genre-based recommendations
✅ Beautiful UI with dark/light mode
✅ Mobile responsive design
✅ Recommendation button for similar movies
✅ Movie detail pages

## 🐛 Troubleshooting

**If deployment fails:**
1. Check that all files are committed to Git
2. Verify `requirements.txt` has all dependencies
3. Check the deployment logs for errors
4. Ensure `final_dataset.csv` is in the repository

**If the app doesn't work:**
1. Check that the CSV file is accessible
2. Verify the port configuration
3. Check the hosting platform's logs

## 📊 Performance Notes

- The app loads all movies into memory on startup
- For large datasets, consider using a database
- Free tiers may have cold start delays
- Consider upgrading for production use

---

**Ready to deploy? Choose your preferred platform and follow the steps above!** 🚀
