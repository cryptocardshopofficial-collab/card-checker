# How to Go Live Instantly with Ngrok

If you want to share your local website with customers RIGHT NOW without deploying to a server, use Ngrok.

## Step 1: Download Ngrok
1. Go to [ngrok.com](https://ngrok.com/download) and download for Windows.
2. Unzip the file.

## Step 2: Connect Your Account
1. Sign up on the website to get your "Authtoken".
2. Open your terminal and run:
   ```bash
   ngrok config add-authtoken YOUR_TOKEN_HERE
   ```

## Step 3: Start the Tunnel
1. Make sure your Python app is running (`python app.py`).
2. Open a **New Terminal** window.
3. Run this command:
   ```bash
   ngrok http 5000
   ```

## Step 4: Share the Link
Ngrok will show you a URL like `https://random-name.ngrok-free.app`.
**Send this link to anyone in the world**, and they will see your website running on your laptop!
