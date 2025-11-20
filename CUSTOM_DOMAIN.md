# Custom Domain Setup Guide

Your portfolio is now configured to work with your custom domain **alifouladgar.com**.

## What I've Done

1. ✅ Updated `astro.config.mjs` to use `https://alifouladgar.com`
2. ✅ Removed the `/my_portfolio_dev` base path
3. ✅ Created `public/CNAME` file with your domain
4. ✅ Pushed changes to GitHub

## Cloudflare DNS Configuration

You need to configure these DNS records in your Cloudflare dashboard:

### Option 1: CNAME Record (Recommended)

1. Go to your Cloudflare dashboard → DNS settings for `alifouladgar.com`
2. Add a new **CNAME** record:
   - **Name**: `@` (or leave blank for root domain)
   - **Target**: `amfooladgar.github.io`
   - **Proxy status**: ⚠️ **DNS only** (turn off the orange cloud for now)
   - **TTL**: Auto

3. If you want **www.alifouladgar.com** to also work:
   - **Name**: `www`
   - **Target**: `amfooladgar.github.io`
   - **Proxy status**: DNS only
   - **TTL**: Auto

### Option 2: A Records (Alternative)

If CNAME doesn't work, use these A records instead:

1. Delete any existing A records for `@`
2. Add these **4 A records** (all with name `@`):
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`

## GitHub Pages Configuration

1. Go to your repository: `https://github.com/amfooladgar/my_portfolio_dev`
2. Go to **Settings** → **Pages**
3. Under **Custom domain**, enter: `alifouladgar.com`
4. Click **Save**
5. ✅ Check **Enforce HTTPS** (after DNS propagates)

## Troubleshooting

### "Not getting the page properly"

If you're seeing issues:

1. **DNS Propagation**: Can take 1-48 hours. Check status at: https://www.whatsmydns.net/#CNAME/alifouladgar.com
2. **Cache**: Clear your browser cache or try incognito mode
3. **Cloudflare Proxy**: Make sure the orange cloud is OFF (DNS only) initially
4. **GitHub Pages**: Verify the custom domain is saved in Settings → Pages

### Once DNS Propagates

After DNS is working (24-48 hours):
- You can turn ON Cloudflare proxy (orange cloud) for DDoS protection and CDN
- Enable HTTPS in both Cloudflare and GitHub Pages

## Expected URLs

- ✅ `https://alifouladgar.com` (primary)
- ✅ `https://www.alifouladgar.com` (if configured)
- ❌ `https://amfooladgar.github.io/my_portfolio_dev` (will redirect)
