# How to Deploy Your Website Online (Free)

To make your website accessible to everyone, we will use **Render.com**. It is free, secure, and very easy to use.

## Step 1: Upload Code to GitHub
You need to put your code on GitHub first.
1. Create an account at [github.com](https://github.com).
2. Create a **New Repository** named `card-checker`.
3. Upload your files (`app.py`, `Procfile`, `requirements.txt`, and the `templates` folder) to this repository.

## Step 2: Deploy on Render
1. Go to [render.com](https://render.com) and sign up (you can use your GitHub account).
2. Click **"New +"** and select **"Web Service"**.
3. Select "Build and deploy from a Git repository".
4. Connect your GitHub account and select your `card-checker` repository.
5. **Configuration**:
   - **Name**: `my-card-checker` (or anything you like)
   - **Region**: Frankfurt (or closest to you)
   - **Branch**: `main`
   - **Runtime**: `Python 3`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `gunicorn app:app`
   - **Instance Type**: Free

6. Click **"Create Web Service"**.

## Step 3: Done!
Render will take about 2-3 minutes to build your site.
Once finished, it will give you a link (e.g., `https://my-card-checker.onrender.com`).
**Share this link with your customers!**
