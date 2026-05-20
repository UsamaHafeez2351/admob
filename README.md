# AdMob App Ads Verification Website

A simple static website for Google AdMob app-ads.txt verification, ready for Vercel deployment.

## 📁 Folder Structure

```
admobproject/
├── index.html      # Main HTML file
├── style.css       # Styling
├── app-ads.txt     # AdMob verification file (MUST be in ROOT)
└── README.md       # This file
```

## 🚀 Deployment Guide

### Step 1: Initialize Git Repository

Open your terminal in the project folder and run:

```bash
git init
git add .
git commit -m "Initial commit: AdMob app-ads.txt verification website"
```

### Step 2: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top-right corner
3. Select **New repository**
4. Enter a repository name (e.g., `admob-verification`)
5. Make it **Public** (recommended for Vercel)
6. Click **Create repository**

### Step 3: Push to GitHub

Copy the commands shown on GitHub after creating the repository. They will look like this:

```bash
git remote add origin https://github.com/YOUR_USERNAME/admob-verification.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### Step 4: Deploy to Vercel

1. Go to [Vercel](https://vercel.com) and sign up/login
2. Click **Add New** → **Project**
3. Click **Import** next to your GitHub repository
4. Configure the project:
   - **Framework Preset**: Other
   - **Root Directory**: `./` (leave as default)
   - **Build Command**: (leave empty)
   - **Output Directory**: `./` (leave as default)
5. Click **Deploy**
6. Wait for deployment to complete (usually takes 30-60 seconds)
7. Your site will be live at: `https://admob-verification.vercel.app`

## ✅ Verify app-ads.txt

After deployment, verify your app-ads.txt file is accessible:

1. Open: `https://your-project-name.vercel.app/app-ads.txt`
2. You should see: `google.com, pub-XXXXXXXXXXXXXXXX, DIRECT, f08c47fec0942fa0`
3. Copy this URL and add it to your AdMob app settings

## 🔄 How to Update app-ads.txt

### Option 1: Via GitHub (Recommended)

1. Edit `app-ads.txt` in your project folder
2. Commit and push changes:
   ```bash
   git add app-ads.txt
   git commit -m "Update app-ads.txt"
   git push
   ```
3. Vercel will automatically redeploy your site

### Option 2: Via Vercel Dashboard

1. Go to your Vercel project dashboard
2. Click **Settings** → **Git**
3. Click **Redeploy** to trigger a new deployment

## 📝 Important Notes

- **app-ads.txt MUST stay in the ROOT folder** - this is critical for AdMob verification
- Replace `pub-XXXXXXXXXXXXXXXX` with your actual AdMob Publisher ID
- The file must be accessible at `https://your-domain.com/app-ads.txt`
- Vercel automatically serves static files from the root directory

## 🔧 Customization

### Update Publisher ID

Edit `app-ads.txt` and replace `pub-XXXXXXXXXXXXXXXX` with your actual AdMob Publisher ID.

Example:
```
google.com, pub-1234567890123456, DIRECT, f08c47fec0942fa0
```

### Change Website Content

Edit `index.html` to modify:
- Heading text
- Subtitle text
- Button link

### Modify Styling

Edit `style.css` to customize:
- Colors
- Fonts
- Layout
- Animations

## 📱 Responsive Design

The website is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones

## 🌐 Vercel Features

- Automatic HTTPS
- Global CDN
- Automatic deployments from Git
- Custom domain support
- Preview deployments

## 🆘 Troubleshooting

### app-ads.txt not accessible

- Ensure the file is in the ROOT folder
- Check the file name is exactly `app-ads.txt` (lowercase)
- Verify Vercel deployment completed successfully

### Deployment failed

- Check your Git repository is properly connected
- Ensure all files are committed and pushed
- Review Vercel deployment logs for errors

### AdMob not verifying

- Wait 24-48 hours after deployment for AdMob to detect the file
- Verify the URL is correct in AdMob settings
- Check the file content matches AdMob requirements

## 📚 Resources

- [AdMob app-ads.txt Guide](https://support.google.com/admob/answer/9883790)
- [Vercel Documentation](https://vercel.com/docs)
- [IAB app-ads.txt Specification](https://iabtechlab.com/standards/app-ads-txt/)

---

**Ready to deploy!** Follow the steps above to get your AdMob verification site live.
