# Deployment Documentation

This folder contains deployment-related documentation and configuration files.

## 📁 Files in Root Directory (Required for Deployment)

These files must be in the root directory for deployment platforms to find them:

- `requirements.txt` - Python dependencies
- `Procfile` - Tells Heroku how to run your app
- `runtime.txt` - Specifies Python version
- `.gitignore` - Excludes unnecessary files from Git

## 🚀 Deployment Platforms

### 1. Railway (Recommended)
- **Easiest setup** - Just connect GitHub and deploy
- **Free tier available**
- **Automatic deployments**

### 2. Render
- **Good alternative** to Railway
- **Free tier available**
- **Manual configuration required**

### 3. Heroku
- **Classic choice** for Flask apps
- **No free tier** (requires credit card)
- **Well-documented**

## 📋 Quick Deployment Steps

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
   - Wait for deployment

3. **Your app will be live!** 🎉

## 🔧 Configuration Files

- `requirements.txt` - Lists all Python packages needed
- `Procfile` - Defines how to start the web server
- `runtime.txt` - Specifies Python version
- `.gitignore` - Excludes files from version control

## 📊 Project Structure

```
Movie-Recommendation-System/
├── movie_recommender.py          # Main Flask application
├── final_dataset.csv            # Movie data
├── templates/                   # HTML templates
│   ├── index.html
│   ├── movie_detail.html
│   └── recommendation.html
├── static/                      # CSS and static files
│   ├── style.css
│   └── appearance.css
├── deployment/                  # Deployment documentation
│   └── README.md
├── requirements.txt             # Python dependencies
├── Procfile                     # Heroku configuration
├── runtime.txt                  # Python version
├── .gitignore                   # Git ignore rules
└── README.md                    # Main project documentation
```

## ⚠️ Important Notes

- The `final_dataset.csv` file is large (200MB+) - make sure it's committed to Git
- Free tiers have limitations (cold starts, memory limits)
- For production, consider upgrading to paid plans
