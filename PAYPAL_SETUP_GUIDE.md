# How to Connect Your PayPal Account

To receive money on this website, you need **API Keys**. You can only get these with a **Business Account** (it's free).

## Step 1: Upgrade Your Account
1. Log in to your existing Personal PayPal account.
2. Go to **Settings** (Gear Icon).
3. Look for **"Upgrade to a Business account"** or **"Sell on PayPal"**.
4. Follow the steps (Use your own name as the "Business Name").

## Step 2: Get the Keys
1. Once upgraded, go to [developer.paypal.com](https://developer.paypal.com).
2. Log in with your same PayPal email/password.
3. Click **"Apps & Credentials"** (Top menu).
4. Toggle to **"Live"** (Not Sandbox).
5. Click **"Create App"**.
6. Name it "Card Checker".
7. Copy the **Client ID** and **Secret**.

## Step 3: Add to Code
Open `app.py` and paste them here:

```python
paypalrestsdk.configure({
  "mode": "live", 
  "client_id": "PASTE_CLIENT_ID_HERE",
  "client_secret": "PASTE_SECRET_HERE"
})
```

## Alternative: PayPal.Me Link
If this is too difficult, we can just use your personal payment link (e.g., `paypal.me/yourname`).
Let me know if you want to switch to this simpler method!
